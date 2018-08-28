---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 0
info:
  title: Digital River Shopper API Get Shoppers Me Orders Shipping Address
  description: Get shoppers me orders shipping address.
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/orders:
    get:
      summary: Get Shoppers Me Orders
      description: Get shoppers me orders.
      operationId: getV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeorders-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
    post:
      summary: Post Shoppers Me Orders
      description: Post shoppers me orders.
      operationId: postV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeorders-post
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
  /v1/shoppers/me/orders/{id}:
    get:
      summary: Get Shoppers Me Orders
      description: Get shoppers me orders.
      operationId: getV1ShoppersMeOrders
      x-api-path-slug: v1shoppersmeordersid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
  /v1/shoppers/me/orders/{id}/billing-address:
    get:
      summary: Get Shoppers Me Orders Billing Address
      description: Get shoppers me orders billing address.
      operationId: getV1ShoppersMeOrdersBillingAddress
      x-api-path-slug: v1shoppersmeordersidbillingaddress-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Billing
      - Ress
  /v1/shoppers/me/orders/{id}/line-items:
    get:
      summary: Get Shoppers Me Orders Line Items
      description: Get shoppers me orders line items.
      operationId: getV1ShoppersMeOrdersLineItems
      x-api-path-slug: v1shoppersmeordersidlineitems-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Line
      - Items
  /v1/shoppers/me/orders/{id}/line-items/{lineItemId}:
    get:
      summary: Get Shoppers Me Orders Line Items Lineitemid
      description: Get shoppers me orders line items lineitemid.
      operationId: getV1ShoppersMeOrdersLineItemsLineitem
      x-api-path-slug: v1shoppersmeordersidlineitemslineitemid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lineItemId
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Line
      - Items
      - Lineitemid
  /v1/shoppers/me/orders/{id}/shipping-address:
    get:
      summary: Get Shoppers Me Orders Shipping Address
      description: Get shoppers me orders shipping address.
      operationId: getV1ShoppersMeOrdersShippingAddress
      x-api-path-slug: v1shoppersmeordersidshippingaddress-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Orders
      - Shipping
      - Ress
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