swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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
    put:
      summary: Put Orders
      description: 'Only ''status'', ''tracking_number'', ''tracking_company'', ''additional_information''
        and ''additional_fields'' are available for update.<br/>Use the JSON format:<br/>''{
        "order": {"status": "Paid", "tracking_company": "other", "tracking_number":
        "123456789", "additional_information": "My custom message.", "additional_fields":
        [{"label": "Gift Name", "value": "Duarte"}, {"label": "Gift Wrapping Color",
        "value": "Green"}]} }}''<br/>or in CURL:<br/>curl -X PUT -d ''{ "order": {"status":
        "Paid", "additional_information": "My custom message."}}'' "https://api.jumpseller.com/v1/orders/{id}.json?login=storecode&authtoken=XXXXX"
        -H "Content-Type:application/json"'
      operationId: putOrders.json
      x-api-path-slug: ordersid-json-put
      parameters:
      - in: body
        name: body
        description: Order parameters to change
        schema:
          $ref: '#/definitions/holder'
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
  /orders/{id}/history.json:
    get:
      summary: Get Orders History
      description: ""
      operationId: getOrdersHistory.json
      x-api-path-slug: ordersidhistory-json-get
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
      - History
      - Json
    post:
      summary: Post Orders History
      description: ""
      operationId: postOrdersHistory.json
      x-api-path-slug: ordersidhistory-json-post
      parameters:
      - in: body
        name: body
        description: Order History parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of the OrderHistory
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Id
      - History
      - Json