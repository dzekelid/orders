swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLastClosingPricesOrdered:
    get:
      summary: Get Last Closing Prices Ordered
      description: Returns last closing price for a collection of securities.
      operationId: postGetlastclosingpricesordered
      x-api-path-slug: getlastclosingpricesordered-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
      - Ordered
  /GetLastClosingPricesOrderedAdjusted:
    get:
      summary: Get Last Closing Prices Ordered Adjusted
      description: Returns last closing price for a collection of securities.This
        include the splits and dividends adjusted price
      operationId: postGetlastclosingpricesorderedadjusted
      x-api-path-slug: getlastclosingpricesorderedadjusted-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
      - Ordered
      - Adjusted