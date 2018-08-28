---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Get Orders
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders.json:
    get:
      summary: Get Orders
      description: ""
      operationId: getOrders.json
      x-api-path-slug: orders-json-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Json
    post:
      summary: Post Orders
      description: 'Use the JSON format:<br/>''{ "order": {"status": "Paid", "shipping_method_id":
        123, "products": [{ "id": 123, "qty": 1}], "customer": {"id": 123}}}''<br/>or
        in CURL:<br/>curl -X POST -d ''{ "order": {"status": "Paid", "shipping_method_id":
        123, "products": [{ "id": 123, "qty": 1}], "customer": {"id": 123}}}'' "https://api.jumpseller.com/v1/orders.json?login=storecode&authtoken=XXXXX"
        -H "Content-Type:application/json"'
      operationId: postOrders.json
      x-api-path-slug: orders-json-post
      parameters:
      - in: body
        name: body
        description: Order parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Json
  /orders/status/{status}.json:
    get:
      summary: Get Orders Status Status
      description: ""
      operationId: getOrdersStatusStatus.json
      x-api-path-slug: ordersstatusstatus-json-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: status
        description: Status of the Order used as filter
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Status
      - Status
      - Json
  /orders/{id}.json:
    get:
      summary: Get Orders
      description: ""
      operationId: getOrders.json
      x-api-path-slug: ordersid-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Order
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Id
      - Json
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