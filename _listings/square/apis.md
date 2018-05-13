---
name: Square
description: Starting with a free credit card reader for the iPhone, iPad, and Android
  devices, Square Reader allows anyone to accept credit cards anywhere, anytime, for
  a low transaction rate of 2.75 percent per swipe, with no hidden fees. Square Register
  serves as a full point-of-sale system for businesses to accept payments, manage
  items, and share menu and location information. Square Wallet, available in the
  US, is the most seamless way to pay, enabling individuals to pay at their favorite
  local businesses, discover new ones nearby, explore menu listings, and store receipts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Payments
- Payment API
- Credit Cards
- Commerce
created: "2018-05-13"
modified: "2018-05-13"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Post V2 Locations Location Orders
  description: |-
    Creates an [Order](#type-order) that can then be referenced as `order_id` in a
    request to the [Charge](#endpoint-charge) endpoint. Orders specify products for
    purchase, along with discounts, taxes, and other settings to apply to the purchase.

    To associate a created order with a request to the Charge endpoint, provide the
    order's `id` in the `order_id` field of your request.

    You cannot modify an order after you create it. If you need to modify an order,
    instead create a new order with modified details.

    To learn more about the Orders API, see the [Orders API Overview](https://docs.connect.squareup.com/articles/orders-api-overview).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/square-logo.png
  humanURL: https://squareup.com
  baseURL: https://connect.squareup.com/v1/
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/square/v2-locations-location-id-orders-post.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---