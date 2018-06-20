---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Partner
  version: "1.0"
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
---