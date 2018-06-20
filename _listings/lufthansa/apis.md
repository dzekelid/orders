---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: Orders
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Partner Orders
  x-api-slug: lh-partner
  description: Retrieve order by ID and optionally name. This service is only accessible
    for LH privileged partners
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//orders/orders/{orderID}/{name}
  tags: Orders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/lufthansa/ordersordersorderidname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/lufthansa/ordersordersorderidname-get-openapi.md
- name: LH Partner
  x-api-slug: lh-partner
  description: Book your flights to Germany, Italy, UK or France online at attractive
    low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/lufthansa/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/lufthansa
- type: x-twitter
  url: https://twitter.com/lufthansa
- type: x-website
  url: http://lufthansa.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---