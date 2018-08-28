---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Get Historical Trades By Specified Order
  description: Get historical trades by specified order.
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
    post:
      summary: Create New Order
      description: Create new order.
      operationId: postOrder
      x-api-path-slug: order-post
      parameters:
      - in: formData
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
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
  /order/{clientOrderId}:
    get:
      summary: Get A Single Order By ClientOrderId
      description: Get a single order by clientorderid.
      operationId: getOrderClientorder
      x-api-path-slug: orderclientorderid-get
      parameters:
      - in: path
        name: clientOrderId
      - in: query
        name: wait
        description: Long polling wait timeout in milliseconds
      responses:
        200:
          description: OK
      tags:
      - Single
      - Order
      - By
      - ClientOrderId
    put:
      summary: Create New Order
      description: Create new order.
      operationId: putOrderClientorder
      x-api-path-slug: orderclientorderid-put
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: expireTime
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: side
      - in: formData
        name: stopPrice
      - in: formData
        name: strictValidate
        description: Strict validate amount and price precision without rounding
      - in: formData
        name: symbol
      - in: formData
        name: timeInForce
      - in: formData
        name: type
      responses:
        200:
          description: OK
      tags:
      - New
      - Order
    delete:
      summary: Cancel Order
      description: Cancel order.
      operationId: deleteOrderClientorder
      x-api-path-slug: orderclientorderid-delete
      parameters:
      - in: path
        name: clientOrderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
    patch:
      summary: Cancel Replace Order
      description: Cancel replace order.
      operationId: patchOrderClientorder
      x-api-path-slug: orderclientorderid-patch
      parameters:
      - in: path
        name: clientOrderId
      - in: formData
        name: price
      - in: formData
        name: quantity
      - in: formData
        name: requestClientId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Replace
      - Order
  /history/order/{id}/trades:
    get:
      summary: Get Historical Trades By Specified Order
      description: Get historical trades by specified order.
      operationId: getHistoryOrderTrades
      x-api-path-slug: historyorderidtrades-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Trades
      - By
      - Specified
      - Order
  /public/orderbook/{symbol}:
    get:
      summary: Orderbook
      description: Orderbook.
      operationId: getPublicOrderbookSymbol
      x-api-path-slug: publicorderbooksymbol-get
      parameters:
      - in: query
        name: limit
        description: 0 - full orderbook otherwise number of levels
      - in: path
        name: symbol
      responses:
        200:
          description: OK
      tags:
      - Orderbook
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