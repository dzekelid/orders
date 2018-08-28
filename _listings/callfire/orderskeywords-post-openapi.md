---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Purchase keywords
  description: Purchase keywords. Send a list of available keywords into this API
    to purchase them using CallFire credits. Make sure the account has enough credits
    before trying to purchase the keywords
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