---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Get Historical Orders
  description: Get historical orders.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order:
    get:
      summary: List Your Current Open Orders
      description: List your current open orders.
      operationId: getOrder
      x-api-path-slug: order-get
      parameters:
      - in: query
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - List
      - Your
      - Current
      - Open
      - Orders
    delete:
      summary: Cancel All Open Orders
      description: Cancel all open orders.
      operationId: deleteOrder
      x-api-path-slug: order-delete
      parameters:
      - in: formData
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - ""
      - Open
      - Orders
  /history/order:
    get:
      summary: Get Historical Orders
      description: Get historical orders.
      operationId: getHistoryOrder
      x-api-path-slug: historyorder-get
      parameters:
      - in: query
        name: clientOrderId
      - in: query
        name: from
        description: Datetime in iso format or timestamp in millisecond
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: symbol
      - in: query
        name: till
        description: Datetime in iso format or timestamp in millisecond
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Orders
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