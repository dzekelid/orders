---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Get Orders Orderid
  description: Get orders orderid.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders:
    get:
      summary: Get Orders
      description: Get orders.
      operationId: getOrders
      x-api-path-slug: orders-get
      parameters:
      - in: query
        name: orderNumber
        description: orderNumber
      - in: query
        name: orderStatus
        description: orderStatus
      responses:
        200:
          description: OK
      tags:
      - Orders
  /orders/summary:
    get:
      summary: Get Orders Summary
      description: Get orders summary.
      operationId: getOrdersSummary
      x-api-path-slug: orderssummary-get
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Summary
  /orders/{orderId}:
    get:
      summary: Get Orders Orderid
      description: Get orders orderid.
      operationId: getOrdersOrder
      x-api-path-slug: ordersorderid-get
      parameters:
      - in: path
        name: orderId
        description: orderId
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Orderid
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