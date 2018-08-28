swagger: "2.0"
x-collection-name: Steem
x-complete: 1
info:
  title: Interactive Steem API
  description: interactive-steem-api-lets-you-interact-with-steem-blockchain-and-make-a-request-get-output-and-start-implementing-new-apps-apis-have-default-parameters-set-to-get-you-started-and-see-how-request-works--api-list-is-compiled-from-steem-githubhttpsgithub-comsteemitsteem-1httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappapi-hpp-and-2httpsgithub-comsteemitsteemtreemasterlibrariesappincludesteemitappdatabase-api-hpp--if-you-want-to-contribute-documenting-detail-of-properties-and-output-contact-goodkarmahttpssteemit-chatdirectgoodkarma--you-can-also-check-full-list-here-steem-jshttpssteemjs-com
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_open_orders:
    get:
      summary: get_open_orders
      description: get_open_orders
      operationId: get-open-orders
      x-api-path-slug: get-open-orders-get
      parameters:
      - in: query
        name: owner
        description: account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Open
      - Orders
  /get_order_book:
    get:
      summary: get_order_book
      description: get_order_book
      operationId: get-order-book
      x-api-path-slug: get-order-book-get
      parameters:
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Order
      - Book