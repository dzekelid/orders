---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Events Orders
  description: Returns a paginated response with a key of orders, containing a list
    of order against this event.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/orders/:
    get:
      summary: Get Events Orders
      description: Returns a paginated response with a key of orders, containing a
        list of order against this event.
      operationId: getEventsOrders
      x-api-path-slug: eventsidorders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return orders changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: last_item_seen
        description: Only return orders changed on or after the time given and with
          an id bigger than last item seen
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: refund_request_statuses
        description: Return only orders with selected refund requests statuses
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), all
          (both) orders and all_not_deleted (active and inactive but not deleted)
          (Valid choices are: active, inactive, all, or all_not_deleted)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
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