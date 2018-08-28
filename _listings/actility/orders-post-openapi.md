---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Core API Order creation
  description: Creates an order, i.e. creates a subscription to a predefined offer
    for an existing subscriber.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /core/v141/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders:
    get:
      summary: Orders retrieval
      description: Retrieves a list of orders existing within authorized scopes. In
        case of a vendor scope, it retrieves all orders allowed by that vendor. In
        case of a subscriber scope, it retrieves all orders performed by that subscriber.
      operationId: retrieves-a-list-of-orders-existing-within-authorized-scopes-in-case-of-a-vendor-scope-it-retrieves-
      x-api-path-slug: orders-get
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Retrieval
    post:
      summary: Order creation
      description: Creates an order, i.e. creates a subscription to a predefined offer
        for an existing subscriber.
      operationId: creates-an-order-ie-creates-a-subscription-to-a-predefined-offer-for-an-existing-subscriber
      x-api-path-slug: orders-post
      parameters:
      - in: body
        name: order
        description: Contents of the order to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: withProcessingStrategyId
        description: Id of a pre-defined data processing strategy
      responses:
        200:
          description: OK
      tags:
      - Order
      - Creation
  /orders/{orderRef}:
    get:
      summary: Order retrieval
      description: Retrieves the order corresponding to the provided order ref, if
        that order is within authorized scopes.
      operationId: retrieves-the-order-corresponding-to-the-provided-order-ref-if-that-order-is-within-authorized-scope
      x-api-path-slug: ordersorderref-get
      parameters:
      - in: path
        name: orderRef
        description: Ref of the order to retrieve
      responses:
        200:
          description: OK
      tags:
      - Order
      - Retrieval
    delete:
      summary: Order cancellation
      description: Cancels all subscriptions related to the provided order ref, if
        that order is within authorized scopes.
      operationId: cancels-all-subscriptions-related-to-the-provided-order-ref-if-that-order-is-within-authorized-scope
      x-api-path-slug: ordersorderref-delete
      parameters:
      - in: path
        name: orderRef
        description: Ref of the order to cancel
      responses:
        200:
          description: OK
      tags:
      - Order
      - Cancellation
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