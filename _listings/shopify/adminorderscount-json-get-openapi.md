---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Count all orders
  description: Count all orders.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders.json:
    get:
      summary: Get all orders from a customer
      description: Get all orders from a customer.
      operationId: getAdminOrders.json
      x-api-path-slug: adminorders-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: customer_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Orders
      - From
      - Customer
  /admin/orders/count.json:
    get:
      summary: Count all orders
      description: Count all orders.
      operationId: getAdminOrdersCount.json
      x-api-path-slug: adminorderscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
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