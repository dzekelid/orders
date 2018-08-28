swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/accounts/{accountId}/orders:
    get:
      summary: Get Orders
      description: |-
        List Orders owned or managed by the partner.

        See _Authentication and Authorization rules_ and
        _List methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.orders.list
      x-api-path-slug: v1accountsaccountidorders-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: query
        name: customId
        description: Filter Orders that match a case-insensitive, partner-specific
          custom id
      - in: query
        name: name
        description: Filter that matches Orders with a `name`, `show`, `season` or
          `episode`that contains the given case-insensitive name
      - in: query
        name: pageSize
        description: See _List methods rules_ for info about this field
      - in: query
        name: pageToken
        description: See _List methods rules_ for info about this field
      - in: query
        name: pphNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: status
        description: Filter Orders that match one of the given status
      - in: query
        name: studioNames
        description: See _List methods rules_ for info about this field
      - in: query
        name: videoIds
        description: Filter Orders that match any of the given `video_id`s
      responses:
        200:
          description: OK
      tags:
      - Order
  /v1/accounts/{accountId}/orders/{orderId}:
    get:
      summary: Get Order
      description: |-
        Get an Order given its id.

        See _Authentication and Authorization rules_ and
        _Get methods rules_ for more information about this method.
      operationId: playmoviespartner.accounts.orders.get
      x-api-path-slug: v1accountsaccountidordersorderid-get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: path
        name: orderId
        description: REQUIRED
      responses:
        200:
          description: OK
      tags:
      - Order