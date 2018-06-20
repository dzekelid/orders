---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Orders Order
  description: Retrieves a Order by id.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/{order_id}:
    get:
      summary: Get Orders Order
      description: Retrieves a Order by id.
      operationId: getOrdersOrder
      x-api-path-slug: ordersorder-id-get
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - Orders
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