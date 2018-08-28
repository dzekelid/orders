---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Set milestone orders
  version: 1.0.0
  description: Set milestone orders.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/milestones/order:
    put:
      summary: Set milestone orders
      description: Set milestone orders.
      operationId: Progression_SetMilestoneOrderBypurchasingRoleIdBymilestoneOrders
      x-api-path-slug: apiprogressionmilestonesorder-put
      parameters:
      - in: body
        name: milestoneOrders
        description: Collection of milestone orders
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: purchasingRoleId
        description: The purchasing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Milestone
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