---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: reverb Post My Orders Selling Order Refund Requests
  description: Post my orders selling order refund requests.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/orders/awaiting_feedback:
    get:
      summary: Get My Orders Awaiting Feedback
      description: List of orders that need feedback
      operationId: getMyOrdersAwaitingFeedback
      x-api-path-slug: myordersawaiting-feedback-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Awaiting
      - Feedback
  /my/orders/buying/all:
    get:
      summary: Get My Orders Buying All
      description: Returns all orders, newest first.
      operationId: getMyOrdersBuyingAll
      x-api-path-slug: myordersbuyingall-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
  /my/orders/buying/unpaid:
    get:
      summary: Get My Orders Buying Unpa
      description: Returns unpaid orders, newest first.
      operationId: getMyOrdersBuyingUnpa
      x-api-path-slug: myordersbuyingunpaid-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Unpaid
  /my/orders/buying/{id}:
    get:
      summary: Get My Orders Buying
      description: Returns order details for a buyer
      operationId: getMyOrdersBuying
      x-api-path-slug: myordersbuyingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Id
  /my/orders/buying/{id}/mark_received:
    post:
      summary: Post My Orders Buying Mark Received
      description: Marks an order as received by the buyer
      operationId: postMyOrdersBuyingMarkReceived
      x-api-path-slug: myordersbuyingidmark-received-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Id
      - Mark
      - Received
  /my/orders/selling/all:
    get:
      summary: Get My Orders Selling All
      description: Get all seller orders, newest first.
      operationId: getMyOrdersSellingAll
      x-api-path-slug: myorderssellingall-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
  /my/orders/selling/awaiting_shipment:
    get:
      summary: Get My Orders Selling Awaiting Shipment
      description: Get seller orders awaiting shipment, newest first.
      operationId: getMyOrdersSellingAwaitingShipment
      x-api-path-slug: myorderssellingawaiting-shipment-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Awaiting
      - Shipment
  /my/orders/selling/buyer_history/{buyer_id}:
    get:
      summary: Get My Orders Selling Buyer History Buyer
      description: Get my orders selling buyer history buyer.
      operationId: getMyOrdersSellingBuyerHistoryBuyer
      x-api-path-slug: myorderssellingbuyer-historybuyer-id-get
      parameters:
      - in: path
        name: buyer_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Buyer
      - History
      - Buyer
      - Id
  /my/orders/selling/unpaid:
    get:
      summary: Get My Orders Selling Unpa
      description: Get unpaid seller orders, newest first.
      operationId: getMyOrdersSellingUnpa
      x-api-path-slug: myorderssellingunpaid-get
      parameters:
      - in: query
        name: created_end_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: created_start_date
        description: Filter by date created in ISO8601 format - e
      - in: query
        name: offset
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: updated_end_date
        description: Filter by date modified in ISO8601 format - e
      - in: query
        name: updated_start_date
        description: Filter by date modified in ISO8601 format - e
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Unpaid
  /my/orders/selling/{id}:
    get:
      summary: Get My Orders Selling
      description: Returns order details for a seller
      operationId: getMyOrdersSelling
      x-api-path-slug: myorderssellingid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
  /my/orders/selling/{id}/mark_picked_up:
    post:
      summary: Post My Orders Selling Mark Picked Up
      description: Post my orders selling mark picked up.
      operationId: postMyOrdersSellingMarkPickedUp
      x-api-path-slug: myorderssellingidmark-picked-up-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Mark
      - Picked
      - Up
  /my/orders/selling/{id}/ship:
    post:
      summary: Post My Orders Selling Ship
      description: Post my orders selling ship.
      operationId: postMyOrdersSellingShip
      x-api-path-slug: myorderssellingidship-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Id
      - Ship
  /my/orders/selling/{order_id}/refund_requests:
    post:
      summary: Post My Orders Selling Order Refund Requests
      description: Post my orders selling order refund requests.
      operationId: postMyOrdersSellingOrderRefundRequests
      x-api-path-slug: myorderssellingorder-idrefund-requests-post
      parameters:
      - in: path
        name: order_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Order
      - Id
      - Refund
      - Requests
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