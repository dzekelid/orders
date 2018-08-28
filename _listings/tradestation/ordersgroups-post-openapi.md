---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Submit Group Order
  description: "Submits a group order such as Bracket and OCO Orders.\n\n#### Order
    Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one of the orders
    is filled\nor partially-filled, then all of the other orders in the group are\ncancelled.\n\n####
    Bracket OCO Orders\nA bracket order is a special instance of an OCO (Order Cancel
    Order).\nBracket orders are used to exit an existing position. They are designed\nto
    limit loss and lock in profit by ???bracketing??? an order with a\nsimultaneous
    stop and limit order.\n\nBracket orders are limited so that the orders are all
    for the same\nsymbol and are on the same side of the market (either all to sell
    or\nall to cover), and they are restricted to closing transactions.\n\nThe reason
    that they follow these rules is because the orders need to be\nable to auto decrement
    when a partial fill occurs with one of the orders.\nFor example, if the customer
    has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
    and the limit order is partially\nfilled for 500 shares, then the customer would
    want the stop to remain\nopen, but it should automatically decrement the order
    to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen a submitted
    order fails, it can be seen in two different ways:\n-\tImmediately rejected during
    submit to the Orders API with a 400 HTTP status code.\n-\tAccepted by the API
    with a 200 HTTP status code, but you will see the order with a status of ???REJ???
    (rejected) when you fetch the Order from the /v2/accounts/{id}/orders API\n\n####
    NOTE\nWhen a group order is submitted, the order execution system treats each
    sibling order as an individual order. Thus, the system does not validate that
    each order has the same Quantity, and currently it is not able to update a bracket
    order as one transaction, instead you must update each order within a bracket.\n\nIn
    order to prevent errors, please validate the data on the client side."
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{account_keys}/orders:
    get:
      summary: Get Account Orders
      description: |-
        Returns the Orders for the given accounts sorted descending, most recent order first.

        #### Stateless Connection
        Since the web-API provides a stateless connection, it only supports fetching the current state of Orders. If it is needed to display the intermediate state changes, it should be executed at client level.
      operationId: getOrdersByAccounts
      x-api-path-slug: accountsaccount-keysorders-get
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: account_keys
        description: 1 or more Account Keys
      - in: query
        name: pageNum
        description: Conveys the page number to return, given a set of orders and
          a page size
      - in: query
        name: pageSize
        description: Conveys the number of order items to return in the request
      - in: query
        name: since
        description: Start Date from which to pull older orders
      responses:
        200:
          description: Successful response
      tags:
      - Account
      - Orders
  /orders/confirm:
    post:
      summary: Confirm Order
      description: |-
        Returns estimated cost and commission information for an order without the order actually being placed. The fields that are returned in the response depend on the order type.
        The following shows the different fields that will be returned.

        **Base Confirmation**  (All confirmations will have these fields)
        * Route
        * Duration
        * Account
        * SummaryMessage
        * OrderConfirmId

        **Equity Confirmation** (Base Confirmation fields + the following)
        * EstimatedPrice
        * EstimatedPriceDisplay
        * EstimatedCost
        * EstimatedCostDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
        * DebitCreditEstimatedCost
        * DebitCreditEstimatedCostDisplay

        **Forex Confirmation** (Base Confirmation fields + the following)
        * BaseCurrency
        * CounterCurrency
        * InitialMarginDisplay

        **Futures Confirmation** (Base Confirmation fields + the following)
        * ProductCurrency
        * AccountCurrency
        * EstimatedCost
        * EstimatedPrice
        * EstimatedPriceDisplay
        * InitialMarginDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
      operationId: postOrderConfirm
      x-api-path-slug: ordersconfirm-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Confirm
      - Order
  /orders:
    post:
      summary: Submit Order
      description: Submits 1 or more orders
      operationId: postOrder
      x-api-path-slug: orders-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Submit
      - Order
  /orders/{order_id}:
    delete:
      summary: Cancel Order
      description: Cancels an open order. You cannot cancel an order that has been
        filled.
      operationId: cancelOrder
      x-api-path-slug: ordersorder-id-delete
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: path
        name: order_id
        description: An existing Order ID
      responses:
        200:
          description: Successful response
      tags:
      - Cancel
      - Order
    put:
      summary: Update Order
      description: |-
        Updates (Cancels & Replaces) an open order. You cannot update an order
        that has been filled.

        Rules:

         | Original order type              | Fields to update                 | Can only change order type to |
         | -------------------------------- | -------------------------------- | ----------------------------- |
         | Limit Orders                     | Quantity, Stop Price             | Market                        |
         | Stop Orders                      | Quantity, Stop Price             | Market                        |
         | Stop Limit Orders                | Quantity, Stop Price, Stop Limit | Market                        |
         | Stop Market Trailing Stop Orders | Quantity                         | Market                        |
         | Trailing Stop Orders             | Offset type and value            | Market                        |
      operationId: cancelReplaceOrder
      x-api-path-slug: ordersorder-id-put
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: order_id
        description: An existing Order ID
      responses:
        200:
          description: Successful response
      tags:
      - Order
  /orders/groups/confirm:
    post:
      summary: Confirm Group Order
      description: |-
        Returns estimated cost and commission information for a group of orders (OCO, BRK) without the orders actually being placed

        **Base Confirmation**  (All confirmations will have these fields)
        * Route
        * Duration
        * Account
        * SummaryMessage
        * OrderConfirmId

        **Equity Confirmation** (Base Confirmation fields + the following)
        * EstimatedPrice
        * EstimatedPriceDisplay
        * EstimatedCost
        * EstimatedCostDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay

        **Forex Confirmation** (Base Confirmation fields + the following)
        * BaseCurrency
        * CounterCurrency
        * InitialMarginDisplay

        **Futures Confirmation** (Base Confirmation fields + the following)
        * ProductCurrency
        * AccountCurrency
        * EstimatedCost
        * EstimatedPrice
        * EstimatedPriceDisplay
        * InitialMarginDisplay
        * EstimatedCommission
        * EstimatedCommissionDisplay
      operationId: postOrderGroupsConfirm
      x-api-path-slug: ordersgroupsconfirm-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Confirm
      - Group
      - Order
  /orders/groups:
    post:
      summary: Submit Group Order
      description: "Submits a group order such as Bracket and OCO Orders.\n\n####
        Order Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one
        of the orders is filled\nor partially-filled, then all of the other orders
        in the group are\ncancelled.\n\n#### Bracket OCO Orders\nA bracket order is
        a special instance of an OCO (Order Cancel Order).\nBracket orders are used
        to exit an existing position. They are designed\nto limit loss and lock in
        profit by ???bracketing??? an order with a\nsimultaneous stop and limit order.\n\nBracket
        orders are limited so that the orders are all for the same\nsymbol and are
        on the same side of the market (either all to sell or\nall to cover), and
        they are restricted to closing transactions.\n\nThe reason that they follow
        these rules is because the orders need to be\nable to auto decrement when
        a partial fill occurs with one of the orders.\nFor example, if the customer
        has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
        and the limit order is partially\nfilled for 500 shares, then the customer
        would want the stop to remain\nopen, but it should automatically decrement
        the order to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen
        a submitted order fails, it can be seen in two different ways:\n-\tImmediately
        rejected during submit to the Orders API with a 400 HTTP status code.\n-\tAccepted
        by the API with a 200 HTTP status code, but you will see the order with a
        status of ???REJ??? (rejected) when you fetch the Order from the /v2/accounts/{id}/orders
        API\n\n#### NOTE\nWhen a group order is submitted, the order execution system
        treats each sibling order as an individual order. Thus, the system does not
        validate that each order has the same Quantity, and currently it is not able
        to update a bracket order as one transaction, instead you must update each
        order within a bracket.\n\nIn order to prevent errors, please validate the
        data on the client side."
      operationId: postOrderGroup
      x-api-path-slug: ordersgroups-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Submit
      - Group
      - Order
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---