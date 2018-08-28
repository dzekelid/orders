---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get all transactions for an order
  description: Get all transactions for an order.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders.json:
    get:
      summary: Get all orders from a customer
      description: Get all orders from a customer.
      operationId: getAdminOrders.json
      x-api-path-slug: adminorders-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: customer_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Orders
      - From
      - Customer
    post:
      summary: Create a pending order with an existing customer
      description: Create a pending order with an existing customer.
      operationId: postAdminOrders.json
      x-api-path-slug: adminorders-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Pending
      - Order
      - Existing
      - Customer
  /admin/orders/count.json:
    get:
      summary: Count all orders
      description: Count all orders.
      operationId: getAdminOrdersCount.json
      x-api-path-slug: adminorderscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Orders
  /admin/orders/4554953422/cancel.json:
    post:
      summary: Canceling an Order
      description: Canceling an order.
      operationId: postAdminOrders4554953422Cancel.json
      x-api-path-slug: adminorders4554953422cancel-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Canceling
      - Order
  /admin/orders/4554953422/close.json:
    post:
      summary: Close a processed order
      description: Close a processed order.
      operationId: postAdminOrders4554953422Close.json
      x-api-path-slug: adminorders4554953422close-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Close
      - Processed
      - Order
  /admin/orders/4602125518/risks.json:
    get:
      summary: Get all Order Risks for an Order
      description: Get all order risks for an order.
      operationId: getAdminOrders4602125518Risks.json
      x-api-path-slug: adminorders4602125518risks-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Order
      - Risksan
      - Order
  /admin/orders/4554953422/events.json:
    get:
      summary: Get all the events from a particular order
      description: Get all the events from a particular order.
      operationId: getAdminOrders4554953422Events.json
      x-api-path-slug: adminorders4554953422events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Events
      - From
      - Particular
      - Order
  /admin/orders/4554953422/transactions/count.json:
    get:
      summary: Get a count of transactions for an order
      description: Get a count of transactions for an order.
      operationId: getAdminOrders4554953422TransactionsCount.json
      x-api-path-slug: adminorders4554953422transactionscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Transactionsan
      - Order
  /admin/orders/4602125518/risks/8609858574.json:
    get:
      summary: Get a single Order Risk
      description: Get a single order risk.
      operationId: getAdminOrders4602125518Risks8609858574.json
      x-api-path-slug: adminorders4602125518risks8609858574-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Order
      - Risk
    put:
      summary: Update an existing risk detail line on an order
      description: Update an existing risk detail line on an order.
      operationId: putAdminOrders4602125518Risks8609858574.json
      x-api-path-slug: adminorders4602125518risks8609858574-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Existing
      - Risk
      - Detail
      - Line
      - "On"
      - Order
  /admin/orders/4495703502/fulfillments.json:
    get:
      summary: Get a list of all fulfillments for an order.
      description: Get a list of all fulfillments for an order..
      operationId: getAdminOrders4495703502Fulfillments.json
      x-api-path-slug: adminorders4495703502fulfillments-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Fulfillmentsan
      - Order
  /admin/orders/4554953422/refunds.json:
    get:
      summary: Get all refunds from a specific order
      description: Get all refunds from a specific order.
      operationId: getAdminOrders4554953422Refunds.json
      x-api-path-slug: adminorders4554953422refunds-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Refunds
      - From
      - Specific
      - Order
    post:
      summary: Create a new refund for an order
      description: Create a new refund for an order.
      operationId: postAdminOrders4554953422Refunds.json
      x-api-path-slug: adminorders4554953422refunds-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Refundan
      - Order
  /admin/orders/4554953422.json:
    get:
      summary: Get a representation of a single order
      description: Get a representation of a single order.
      operationId: getAdminOrders4554953422.json
      x-api-path-slug: adminorders4554953422-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Representation
      - Single
      - Order
    put:
      summary: Update an order
      description: Update an order.
      operationId: putAdminOrders4554953422.json
      x-api-path-slug: adminorders4554953422-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Order
    delete:
      summary: Delete an order.
      description: Delete an order..
      operationId: deleteAdminOrders4554953422.json
      x-api-path-slug: adminorders4554953422-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Order
  /admin/orders/4554953422/open.json:
    post:
      summary: Re-opening a closed Order
      description: Re-opening a closed order.
      operationId: postAdminOrders4554953422Open.json
      x-api-path-slug: adminorders4554953422open-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Re-opening
      - Closed
      - Order
  /admin/orders/4554953422/transactions.json:
    get:
      summary: Get all transactions for an order
      description: Get all transactions for an order.
      operationId: getAdminOrders4554953422Transactions.json
      x-api-path-slug: adminorders4554953422transactions-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Transactionsan
      - Order
    post:
      summary: Capture a previously authorized order for the full amount
      description: Capture a previously authorized order for the full amount.
      operationId: postAdminOrders4554953422Transactions.json
      x-api-path-slug: adminorders4554953422transactions-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Capture
      - Previously
      - Authorized
      - Orderthe
      - Full
      - Amount
  /admin/orders/4528049998/fulfillments/count.json:
    get:
      summary: Count all the total number of fulfillments for an order.
      description: Count all the total number of fulfillments for an order..
      operationId: getAdminOrders4528049998FulfillmentsCount.json
      x-api-path-slug: adminorders4528049998fulfillmentscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Total
      - Number
      - Fulfillmentsan
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