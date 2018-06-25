---
name: Jumpseller
x-slug: jumpseller
description: We founded Jumpseller.com in 2009 in Europe  we called it Vendder back
  then  and released our first version of the Jumpseller product in September 2010.
  After releasing the product we quickly grew to thousands of customers. In November
  2010, we recei...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
x-kinRank: "7"
x-alexaRank: "153745"
tags: Orders
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/apis.md
specificationVersion: "0.14"
apis:
- name: Jumpseller Get Orders
  x-api-slug: jumpseller
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders.json
  tags: Orders,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/orders-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/orders-json-get-openapi.md
- name: Jumpseller Post Orders
  x-api-slug: jumpseller
  description: 'Use the JSON format:<br/>''{ "order": {"status": "Paid", "shipping_method_id":
    123, "products": [{ "id": 123, "qty": 1}], "customer": {"id": 123}}}''<br/>or
    in CURL:<br/>curl -X POST -d ''{ "order": {"status": "Paid", "shipping_method_id":
    123, "products": [{ "id": 123, "qty": 1}], "customer": {"id": 123}}}'' "https://api.jumpseller.com/v1/orders.json?login=storecode&authtoken=XXXXX"
    -H "Content-Type:application/json"'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders.json
  tags: Orders,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/orders-json-post-openapi.md
- name: Jumpseller Get Orders Status Status
  x-api-slug: jumpseller
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders/status/{status}.json
  tags: Orders,Status,Status,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersstatusstatus-json-get-openapi.md
- name: Jumpseller Get Orders
  x-api-slug: jumpseller
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders/{id}.json
  tags: Orders,Id,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersid-json-get-openapi.md
- name: Jumpseller Put Orders
  x-api-slug: jumpseller
  description: 'Only ''status'', ''tracking_number'', ''tracking_company'', ''additional_information''
    and ''additional_fields'' are available for update.<br/>Use the JSON format:<br/>''{
    "order": {"status": "Paid", "tracking_company": "other", "tracking_number": "123456789",
    "additional_information": "My custom message.", "additional_fields": [{"label":
    "Gift Name", "value": "Duarte"}, {"label": "Gift Wrapping Color", "value": "Green"}]}
    }}''<br/>or in CURL:<br/>curl -X PUT -d ''{ "order": {"status": "Paid", "additional_information":
    "My custom message."}}'' "https://api.jumpseller.com/v1/orders/{id}.json?login=storecode&authtoken=XXXXX"
    -H "Content-Type:application/json"'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders/{id}.json
  tags: Orders,Id,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersid-json-put-openapi.md
- name: Jumpseller Get Orders History
  x-api-slug: jumpseller
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders/{id}/history.json
  tags: Orders,Id,History,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersidhistory-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersidhistory-json-get-openapi.md
- name: Jumpseller Post Orders History
  x-api-slug: jumpseller
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1//orders/{id}/history.json
  tags: Orders,Id,History,Json
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/ordersidhistory-json-post-openapi.md
- name: Jumpseller
  x-api-slug: jumpseller
  description: We founded Jumpseller.com in 2009 in Europe  we called it Vendder back
    then  and released our first version of the Jumpseller product in September 2010.
    After releasing the product we quickly grew to thousands of customers. In November
    2010, we recei...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28432-jumpseller-api.jpg
  humanURL: http://jumpseller.com
  baseURL: https://api.jumpseller.com//v1
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/jumpseller/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/vendder
- type: x-email
  url: info@jumpseller.com
- type: x-email
  url: support@jumpseller.com
- type: x-twitter
  url: https://twitter.com/Jumpseller
- type: x-website
  url: http://jumpseller.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---