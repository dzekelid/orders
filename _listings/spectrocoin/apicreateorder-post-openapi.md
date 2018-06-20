---
swagger: "2.0"
x-collection-name: SpectroCoin
x-complete: 0
info:
  title: Spectro Coin Merchant Create merchant order
  description: Create merchant order
  contact:
    name: info@spectrocoin.com
  version: 1.0.0
host: spectrocoin.com
basePath: /api/merchant/1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/createOrder:
    post:
      summary: Create merchant order
      description: Create merchant order
      operationId: createOrder
      x-api-path-slug: apicreateorder-post
      parameters:
      - in: body
        name: body
        description: Request to create order
        schema:
          $ref: '#/definitions/holder'
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