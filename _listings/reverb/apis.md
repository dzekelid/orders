---
name: Reverb
x-slug: reverb
description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
  was created to find and connect the rich associations between words, ideas, content,
  and people. Through our products, we enhance broader knowledge around favorite topics
  by surfacing interesting information readers might not uncover on their own. We
  make tools for content understanding at every level from the single word on up.
  Wordnik: Get a full view of any word you???re interested in, with definitions, example
  sentences, related words, tweets from Twitter, pictures from Flickr, and much more.Reverb
  for Publishers: Reverb for Publishers brings relevant content to web audiences and
  surfaces additional content for publishers.Reverb for Developers: Reverb is committed
  to the open-source community and is proudly contributing infrastructure software
  to power applications and enterprises both small and gigantic. Our involvement with
  the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Orders
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/apis.md
specificationVersion: "0.14"
apis:
- name: reverb Get My Orders Awaiting Feedback
  x-api-slug: reverb
  description: List of orders that need feedback
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/awaiting_feedback
  tags: My,Orders,Awaiting,Feedback
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersawaiting-feedback-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersawaiting-feedback-get-openapi.md
- name: reverb Get My Orders Buying All
  x-api-slug: reverb
  description: Returns all orders, newest first.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/buying/all
  tags: My,Orders,Buying
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingall-get-openapi.md
- name: reverb Get My Orders Buying Unpa
  x-api-slug: reverb
  description: Returns unpaid orders, newest first.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/buying/unpaid
  tags: My,Orders,Buying,Unpaid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingunpaid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingunpaid-get-openapi.md
- name: reverb Get My Orders Buying
  x-api-slug: reverb
  description: Returns order details for a buyer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/buying/{id}
  tags: My,Orders,Buying,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingid-get-openapi.md
- name: reverb Post My Orders Buying Mark Received
  x-api-slug: reverb
  description: Marks an order as received by the buyer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/buying/{id}/mark_received
  tags: My,Orders,Buying,Id,Mark,Received
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingidmark-received-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingidmark-received-post-openapi.md
- name: reverb Get My Orders Selling All
  x-api-slug: reverb
  description: Get all seller orders, newest first.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/all
  tags: My,Orders,Selling
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingall-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingall-get-openapi.md
- name: reverb Get My Orders Selling Awaiting Shipment
  x-api-slug: reverb
  description: Get seller orders awaiting shipment, newest first.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/awaiting_shipment
  tags: My,Orders,Selling,Awaiting,Shipment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingawaiting-shipment-get-openapi.md
- name: reverb Get My Orders Selling Buyer History Buyer
  x-api-slug: reverb
  description: Get my orders selling buyer history buyer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/buyer_history/{buyer_id}
  tags: My,Orders,Selling,Buyer,History,Buyer,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingbuyer-historybuyer-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingbuyer-historybuyer-id-get-openapi.md
- name: reverb Get My Orders Selling Unpa
  x-api-slug: reverb
  description: Get unpaid seller orders, newest first.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/unpaid
  tags: My,Orders,Selling,Unpaid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingunpaid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingunpaid-get-openapi.md
- name: reverb Get My Orders Selling
  x-api-slug: reverb
  description: Returns order details for a seller
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/{id}
  tags: My,Orders,Selling,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingid-get-openapi.md
- name: reverb Post My Orders Selling Mark Picked Up
  x-api-slug: reverb
  description: Post my orders selling mark picked up.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/{id}/mark_picked_up
  tags: My,Orders,Selling,Id,Mark,Picked,Up
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingidmark-picked-up-post-openapi.md
- name: reverb Post My Orders Selling Ship
  x-api-slug: reverb
  description: Post my orders selling ship.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/{id}/ship
  tags: My,Orders,Selling,Id,Ship
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingidship-post-openapi.md
- name: reverb Post My Orders Selling Order Refund Requests
  x-api-slug: reverb
  description: Post my orders selling order refund requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/selling/{order_id}/refund_requests
  tags: My,Orders,Selling,Order,Id,Refund,Requests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myorderssellingorder-idrefund-requests-post-openapi.md
- name: reverb Get Orders Order Feedback Buyer
  x-api-slug: reverb
  description: Feedback details for an order's buyer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//orders/{order_id}/feedback/buyer
  tags: Orders,Order,Id,Feedback,Buyer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/ordersorder-idfeedbackbuyer-get-openapi.md
- name: reverb Post Orders Order Feedback Buyer
  x-api-slug: reverb
  description: Add feedback about an order's buyer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//orders/{order_id}/feedback/buyer
  tags: Orders,Order,Id,Feedback,Buyer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/ordersorder-idfeedbackbuyer-post-openapi.md
- name: reverb Get Orders Order Feedback Seller
  x-api-slug: reverb
  description: Feedback details for an order's seller
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//orders/{order_id}/feedback/seller
  tags: Orders,Order,Id,Feedback,Seller
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/ordersorder-idfeedbackseller-get-openapi.md
- name: reverb Post Orders Order Feedback Seller
  x-api-slug: reverb
  description: Add feedback about an order's seller
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//orders/{order_id}/feedback/seller
  tags: Orders,Order,Id,Feedback,Seller
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/ordersorder-idfeedbackseller-post-openapi.md
- name: reverb Get My Orders Buying Buying History Seller
  x-api-slug: reverb
  description: Get my orders buying buying history seller.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/orders/buying/buying_history/{seller_id}
  tags: My,Orders,Buying,Buying,History,Seller,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingbuying-historyseller-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/myordersbuyingbuying-historyseller-id-get-openapi.md
- name: reverb
  x-api-slug: reverb
  description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
    was created to find and connect the rich associations between words, ideas, content,
    and people. Through our products, we enhance broader knowledge around favorite
    topics by surfacing interesting information readers might not uncover on their
    own. We make tools for content understanding at every level from the single word
    on up. Wordnik: Get a full view of any word you???re interested in, with definitions,
    example sentences, related words, tweets from Twitter, pictures from Flickr, and
    much more.Reverb for Publishers: Reverb for Publishers brings relevant content
    to web audiences and surfaces additional content for publishers.Reverb for Developers:
    Reverb is committed to the open-source community and is proudly contributing infrastructure
    software to power applications and enterprises both small and gigantic. Our involvement
    with the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reverb/openapi.md
x-common:
- type: x-blog
  url: http://blog.helloreverb.com/
- type: x-blog-rss
  url: http://blog.helloreverb.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/reverb-technologies
- type: x-github
  url: https://github.com/reverb
- type: x-twitter
  url: https://twitter.com/reverb
- type: x-website
  url: https://helloreverb.com/app
- type: x-website
  url: http://reverb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---