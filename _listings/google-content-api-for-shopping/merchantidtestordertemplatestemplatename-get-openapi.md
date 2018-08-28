---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Get Test Order
  description: Sandbox only. Retrieves an order template that can be used to quickly
    create a new order in sandbox. This method can only be called for non-multi-client
    accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/batch:
    post:
      summary: Orders
      description: Retrieves or modifies multiple orders in a single request. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.custombatch
      x-api-path-slug: ordersbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
  /{merchantId}/orders:
    get:
      summary: Get Orders
      description: Lists the orders in your Merchant Center account. This method can
        only be called for non-multi-client accounts.
      operationId: content.orders.list
      x-api-path-slug: merchantidorders-get
      parameters:
      - in: query
        name: acknowledged
        description: Obtains orders that match the acknowledgement status
      - in: query
        name: maxResults
        description: The maximum number of orders to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: orderBy
        description: The ordering of the returned list
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: query
        name: placedDateEnd
        description: Obtains orders placed before this date (exclusively), in ISO
          8601 format
      - in: query
        name: placedDateStart
        description: Obtains orders placed after this date (inclusively), in ISO 8601
          format
      - in: query
        name: statuses
        description: Obtains orders that match any of the specified statuses
      responses:
        200:
          description: OK
      tags:
      - Orders
  /{merchantId}/orders/{orderId}:
    get:
      summary: Get Order
      description: Retrieves an order from your Merchant Center account. This method
        can only be called for non-multi-client accounts.
      operationId: content.orders.get
      x-api-path-slug: merchantidordersorderid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Order
  /{merchantId}/orders/{orderId}/acknowledge:
    post:
      summary: Acknowledge Order
      description: Marks an order as acknowledged. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.acknowledge
      x-api-path-slug: merchantidordersorderidacknowledge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Order
  /{merchantId}/orders/{orderId}/cancel:
    post:
      summary: Cancel Order
      description: Cancels all line items in an order. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.cancel
      x-api-path-slug: merchantidordersorderidcancel-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to cancel
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
  /{merchantId}/orders/{orderId}/cancelLineItem:
    post:
      summary: Cancel Order Line Item
      description: Cancels a line item. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.cancellineitem
      x-api-path-slug: merchantidordersorderidcancellineitem-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
      - Line
      - Item
  /{merchantId}/orders/{orderId}/refund:
    post:
      summary: Refund Order
      description: Refund a portion of the order, up to the full amount paid. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.refund
      x-api-path-slug: merchantidordersorderidrefund-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order to refund
      responses:
        200:
          description: OK
      tags:
      - Refund
      - Order
  /{merchantId}/orders/{orderId}/updateMerchantOrderId:
    post:
      summary: Update Merchant Order ID
      description: Updates the merchant order ID for a given order. This method can
        only be called for non-multi-client accounts.
      operationId: content.orders.updatemerchantorderid
      x-api-path-slug: merchantidordersorderidupdatemerchantorderid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - Merchant
      - Order
      - ID
  /{merchantId}/orders/{orderId}/updateShipment:
    post:
      summary: Update order Shippment
      description: Updates a shipment's status, carrier, and/or tracking ID. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.updateshipment
      x-api-path-slug: merchantidordersorderidupdateshipment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the order
      responses:
        200:
          description: OK
      tags:
      - order
      - Shippment
  /{merchantId}/ordersbymerchantid/{merchantOrderId}:
    get:
      summary: Get Order
      description: Retrieves an order using merchant order id. This method can only
        be called for non-multi-client accounts.
      operationId: content.orders.getbymerchantorderid
      x-api-path-slug: merchantidordersbymerchantidmerchantorderid-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: merchantOrderId
        description: The merchant order id to be looked for
      responses:
        200:
          description: OK
      tags:
      - Order
  /{merchantId}/testorders:
    post:
      summary: Create Test Order
      description: Sandbox only. Creates a test order. This method can only be called
        for non-multi-client accounts.
      operationId: content.orders.createtestorder
      x-api-path-slug: merchantidtestorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: merchantId
        description: The ID of the managing account
      responses:
        200:
          description: OK
      tags:
      - Test
      - Order
  /{merchantId}/testorders/{orderId}/advance:
    post:
      summary: Update Test Order
      description: Sandbox only. Moves a test order from state "inProgress" to state
        "pendingShipment". This method can only be called for non-multi-client accounts.
      operationId: content.orders.advancetestorder
      x-api-path-slug: merchantidtestordersorderidadvance-post
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: orderId
        description: The ID of the test order to modify
      responses:
        200:
          description: OK
      tags:
      - Test
      - Order
  /{merchantId}/testordertemplates/{templateName}:
    get:
      summary: Get Test Order
      description: Sandbox only. Retrieves an order template that can be used to quickly
        create a new order in sandbox. This method can only be called for non-multi-client
        accounts.
      operationId: content.orders.gettestordertemplate
      x-api-path-slug: merchantidtestordertemplatestemplatename-get
      parameters:
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: path
        name: templateName
        description: The name of the template to retrieve
      responses:
        200:
          description: OK
      tags:
      - Test
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