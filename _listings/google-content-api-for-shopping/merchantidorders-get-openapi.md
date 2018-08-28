---
swagger: "2.0"
x-collection-name: Google Content API for Shopping
x-complete: 0
info:
  title: Google Content API for Shopping API Get Orders
  description: Lists the orders in your Merchant Center account. This method can only
    be called for non-multi-client accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /content/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/batch:
    post:
      summary: Orders
      description: Retrieves or modifies multiple orders in a single request. This
        method can only be called for non-multi-client accounts.
      operationId: content.orders.custombatch
      x-api-path-slug: ordersbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
  /{merchantId}/orders:
    get:
      summary: Get Orders
      description: Lists the orders in your Merchant Center account. This method can
        only be called for non-multi-client accounts.
      operationId: content.orders.list
      x-api-path-slug: merchantidorders-get
      parameters:
      - in: query
        name: acknowledged
        description: Obtains orders that match the acknowledgement status
      - in: query
        name: maxResults
        description: The maximum number of orders to return in the response, used
          for paging
      - in: path
        name: merchantId
        description: The ID of the managing account
      - in: query
        name: orderBy
        description: The ordering of the returned list
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: query
        name: placedDateEnd
        description: Obtains orders placed before this date (exclusively), in ISO
          8601 format
      - in: query
        name: placedDateStart
        description: Obtains orders placed after this date (inclusively), in ISO 8601
          format
      - in: query
        name: statuses
        description: Obtains orders that match any of the specified statuses
      responses:
        200:
          description: OK
      tags:
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