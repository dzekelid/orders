swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/History/limit/order:
    get:
      summary: Get API History Limit Order
      description: Get api history limit order.
      operationId: ApiHistoryLimitOrderGet
      x-api-path-slug: apihistorylimitorder-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - History
      - Limit
      - Order
  /api/OrderBook/{id}:
    get:
      summary: Get API Orderbook
      description: Get api orderbook.
      operationId: ApiOrderBookByIdGet
      x-api-path-slug: apiorderbookid-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Orderbook
  /api/HotWallet/limitOrder:
    post:
      summary: Add API Hotwallet Limitorder
      description: Add api hotwallet limitorder.
      operationId: LimitOrder
      x-api-path-slug: apihotwalletlimitorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Limitorder
  /api/HotWallet/marketOrder:
    post:
      summary: Add API Hotwallet Marketorder
      description: Add api hotwallet marketorder.
      operationId: MarketOrder
      x-api-path-slug: apihotwalletmarketorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SignatureVerificationToken
        description: signature verification token
      responses:
        200:
          description: OK
      tags:
      - Hotwallet
      - Marketorder
  /api/SettingSignOrder:
    post:
      summary: Add API Settingsignorder
      description: Add api settingsignorder.
      operationId: ApiSettingSignOrderPost
      x-api-path-slug: apisettingsignorder-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Settingsignorder