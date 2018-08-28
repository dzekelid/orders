---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Provides comprehensive information for a single online
    store order, including the order's history.
  description: Provides comprehensive information for a single online store order,
    including the order's history.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/orders:
    get:
      summary: Provides summary information for a merchant's online store orders.
      description: Provides summary information for a merchant's online store orders.
      operationId: ListOrders
      x-api-path-slug: v1location-idorders-get
      parameters:
      - in: query
        name: batch_token
        description: A pagination cursor to retrieve the next set of results for youroriginal
          query to the endpoint
      - in: query
        name: limit
        description: The maximum number of payments to return in a single response
      - in: path
        name: location_id
        description: The ID of the location to list online store orders for
      - in: query
        name: order
        description: TThe order in which payments are listed in the response
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Informationa
      - Merchants
      - Online
      - Store
      - Orders
  /v1/{location_id}/orders/{order_id}:
    get:
      summary: Provides comprehensive information for a single online store order,
        including the order's history.
      description: Provides comprehensive information for a single online store order,
        including the order's history.
      operationId: RetrieveOrder
      x-api-path-slug: v1location-idordersorder-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Online
      - Store
      - Order
      - ""
      - Including
      - Orders
      - History
    put:
      summary: 'Updates the details of an online store order. Every update you perform
        on an order corresponds to one of three actions:'
      description: 'Updates the details of an online store order. Every update you
        perform on an order corresponds to one of three actions:'
      operationId: UpdateOrder
      x-api-path-slug: v1location-idordersorder-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - S
      - Details
      - Of
      - Online
      - Store
      - Order
      - ""
      - Every
      - Update
      - You
      - Perform
      - "On"
      - Order
      - Corresponds
      - To
      - Of
      - Three
      - 'Actions:'
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