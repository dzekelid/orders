swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/keywords:
    post:
      summary: Purchase keywords
      description: Purchase keywords. Send a list of available keywords into this
        API to purchase them using CallFire credits. Make sure the account has enough
        credits before trying to purchase the keywords
      operationId: orderKeywords
      x-api-path-slug: orderskeywords-post
      parameters:
      - in: body
        name: body
        description: Request object which contains a list of keywords to buy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Keywords
  /orders/numbers:
    post:
      summary: Purchase numbers
      description: Purchase numbers. There are many ways to purchase a number. Set
        either 'tollFreeCount' or 'localCount' along with some querying fields to
        purchase numbers by bulk query. Set the list of numbers to purchase by list.
        Available numbers will be purchased using CallFire credits owned by the user.
        Make sure the account has enough credits before trying to purchase
      operationId: orderNumbers
      x-api-path-slug: ordersnumbers-post
      parameters:
      - in: body
        name: body
        description: 'Request object contains a list of numbers to buy, you can filter
          the numbers by their region information: city, state, zipcode, LATA, etc'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Numbers
  /orders/{id}:
    get:
      summary: Find a specific order
      description: Returns a single NumberOrder instance for a given order id. Order
        contains information about purchased keywords, local, toll-free numbers
      operationId: getOrder
      x-api-path-slug: ordersid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of an order
      responses:
        200:
          description: OK
      tags:
      - Orders