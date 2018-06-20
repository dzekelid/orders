---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
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
---