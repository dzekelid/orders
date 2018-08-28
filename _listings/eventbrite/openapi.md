swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /orders/{id}/:
    get:
      summary: Get Orders
      description: Gets an order by ID an order object.
      operationId: getOrders
      x-api-path-slug: ordersid-get
      responses:
        200:
          description: OK
      tags:
      - Orders
  /users/{id}/orders/:
    get:
      summary: Get Users Orders
      description: Returns a paginated response of orders, under the key orders, of
        all orders the user has placed (i.e. where the user was the person buying
        the tickets).
      operationId: getUsersOrders
      x-api-path-slug: usersidorders-get
      parameters:
      - in: query
        name: '&#160;'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Orders
  /users/{id}/owned_event_orders/:
    get:
      summary: Get Users Owned Event Orders
      description: |-
        Returns a paginated response of orders,
        under the key orders, of orders placed against any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventOrders
      x-api-path-slug: usersidowned-event-orders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), or all
          (both) orders (Valid choices are: active, inactive, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Orders