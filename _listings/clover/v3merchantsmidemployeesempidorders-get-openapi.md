---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all orders for an employee
  version: 1.0.0
  description: Get all orders for an employee.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/orders:
    get:
      summary: Gets a list of orders
      description: Returns a list of orders. See https://docs.clover.com/build/working-with-orders/
        for more details.
      operationId: GetOrders
      x-api-path-slug: v3merchantsmidorders-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, serviceCharge, discounts, credits,
          payments, refunds]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
  /v3/merchants/{mId}/employees/{empId}/orders:
    get:
      summary: Get all orders for an employee
      description: Get all orders for an employee.
      operationId: GetEmployeeOrders
      x-api-path-slug: v3merchantsmidemployeesempidorders-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: query
        name: filter
        description: 'Filter fields: [lineItems, customers, payments, credits, refunds,
          serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
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