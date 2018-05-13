---
swagger: "2.0"
info:
  title: Etsy Get Orders Order Receipts
  description: Retrieves a set of Receipt objects associated to a Order.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/{order_id}/receipts:
    get:
      summary: Get Orders Order Receipts
      description: Retrieves a set of Receipt objects associated to a Order
      operationId: getOrdersOrderReceipts
      responses:
        200:
          description: OK
      tags:
      - orders
      - order
      - receipts
definitions: []
x-collection-name: Etsy
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