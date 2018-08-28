---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_order_book
  description: get_order_book
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_open_orders:
    get:
      summary: get_open_orders
      description: get_open_orders
      operationId: get-open-orders
      x-api-path-slug: get-open-orders-get
      parameters:
      - in: query
        name: owner
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Open
      - Orders
  /get_order_book:
    get:
      summary: get_order_book
      description: get_order_book
      operationId: get-order-book
      x-api-path-slug: get-order-book-get
      parameters:
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Order
      - Book
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