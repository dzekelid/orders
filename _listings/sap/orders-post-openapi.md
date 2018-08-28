---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Creates an order
  description: |-
    Creates an order for the part for which the customer and the supplier haven been colloabrating
    The order is based on the confirmed production option and pricing.
    The login user must be from the customer.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders:
    post:
      summary: Creates an order
      description: |-
        Creates an order for the part for which the customer and the supplier haven been colloabrating
        The order is based on the confirmed production option and pricing.
        The login user must be from the customer.
      operationId: creates-an-order-for-the-part-for-which-the-customer-and-the-supplier-haven-been-colloabratingthe-or
      x-api-path-slug: orders-post
      parameters:
      - in: body
        name: OrderRequest
        description: A request about an order
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Order
  /orders/{orderNumber}/history:
    post:
      summary: Adds a record to the order history
      description: "Adds a record to the history of an order.   \nThe order number
        is sent in the message body of the Order Created event.  \nThe login user
        must be from the additive manufacturing supplier."
      operationId: adds-a-record-to-the-history-of-an-order---the-order-number-is-sent-in-the-message-body-of-the-order
      x-api-path-slug: ordersordernumberhistory-post
      parameters:
      - in: body
        name: OrderItemRequest
        description: A request about an order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderNumber
        description: An order number
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Record
      - To
      - Order
      - History
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