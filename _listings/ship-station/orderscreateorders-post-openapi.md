---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Create/Update Multiple Orders
  description: |-
    This endpoint can be used to create or update multiple orders in one request. If the ``orderKey`` is specified in an order, the existing order with that key will be updated. Note: Only orders in an open status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``) can be updated through this method. ``cancelled`` and ``shipped`` are locked from modification through the API.

    Data Type          |Description
    -------------------|-------------------
    Order, required | An array of [**Order**](http://www.shipstation.com/developer-api/#/reference/model-order) objects (maximum of 100 per request)
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders:
    get:
      summary: List Orders w/o parameters
      description: ""
      operationId: orders.get
      x-api-path-slug: orders-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - W
      - O
      - Parameters
  /orders/createorders:
    post:
      summary: Create/Update Multiple Orders
      description: |-
        This endpoint can be used to create or update multiple orders in one request. If the ``orderKey`` is specified in an order, the existing order with that key will be updated. Note: Only orders in an open status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``) can be updated through this method. ``cancelled`` and ``shipped`` are locked from modification through the API.

        Data Type          |Description
        -------------------|-------------------
        Order, required | An array of [**Order**](http://www.shipstation.com/developer-api/#/reference/model-order) objects (maximum of 100 per request)
      operationId: orders.createorders.post
      x-api-path-slug: orderscreateorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Multiple
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