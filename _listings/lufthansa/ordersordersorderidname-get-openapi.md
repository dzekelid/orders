---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Partner Orders
  version: "1.0"
  description: Retrieve order by ID and optionally name. This service is only accessible
    for LH privileged partners
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/orders/{orderID}/{name}:
    get:
      summary: Orders
      description: Retrieve order by ID and optionally name. This service is only
        accessible for LH privileged partners
      operationId: Orders
      x-api-path-slug: ordersordersorderidname-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: name
        description: Surname of traveller
      - in: path
        name: orderID
        description: Unique order identifier
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