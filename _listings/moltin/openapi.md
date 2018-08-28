swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/orders:
    get:
      summary: Get all orders
      description: Get all orders.
      operationId: V2OrdersGet
      x-api-path-slug: v2orders-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Orders
  /v2/orders/{orderID}:
    get:
      summary: Get a single order
      description: Get a single order.
      operationId: V2OrdersByOrderIDGet
      x-api-path-slug: v2ordersorderid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Single
      - Order
    put:
      summary: Update an order
      description: |-
        Transactions are created and updated automatically whenever you make a payment request. When a payment is successful, the transaction ID returned from the gateway will be attached to the transaction.

        It is possible for an order to have more than one transaction attached as each attempted payment will be created as a new transaction.
      operationId: V2OrdersByOrderIDPut
      x-api-path-slug: v2ordersorderid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
  /orders/{orderID}/items:
    get:
      summary: Get Order Items
      description: Get order items.
      operationId: OrdersItemsByOrderIDGet
      x-api-path-slug: ordersorderiditems-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: orderID
      responses:
        200:
          description: Successful response
      tags:
      - Order
      - Items