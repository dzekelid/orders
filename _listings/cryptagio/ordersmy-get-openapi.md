---
swagger: "2.0"
x-collection-name: Cryptagio
x-complete: 0
info:
  title: Cryptagio GetMy  Orders
  description: Trades are sorted in reverse creation order.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/my:
    get:
      summary: GetMy  Orders
      description: Trades are sorted in reverse creation order.
      operationId: getOrdersMy
      x-api-path-slug: ordersmy-get
      parameters:
      - in: query
        name: from_time
        description: Filter trades by time
      - in: query
        name: from_uuid
        description: Filter orders by id
      - in: query
        name: limit
        description: Limit the number of returned trades
      - in: query
        name: market
        description: Filter orders by market
      - in: query
        name: order
        description: If set, returned orders will be sorted in specific order
      - in: query
        name: side
        description: Filter orders by side
      - in: query
        name: status
        description: Filter orders by status
      - in: query
        name: to_time
        description: Filter trades by time
      - in: query
        name: type
        description: Filter orders by type
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Orders
      - My
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