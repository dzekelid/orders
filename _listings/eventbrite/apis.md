---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite brings people together through live experiences. Discover
  events that match your passions, or create your own with online ticketing tools.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
x-kinRank: "9"
x-alexaRank: "643"
tags: Orders
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Get Events Orders
  x-api-slug: eventbrite
  description: Returns a paginated response with a key of orders, containing a list
    of order against this event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///events/{id}/orders/
  tags: Events,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/eventsidorders-get-openapi.md
- name: Eventbrite Get Orders
  x-api-slug: eventbrite
  description: Gets an order by ID an order object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///orders/{id}/
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/ordersid-get-openapi.md
- name: Eventbrite Get Users Orders
  x-api-slug: eventbrite
  description: Returns a paginated response of orders, under the key orders, of all
    orders the user has placed (i.e. where the user was the person buying the tickets).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/orders/
  tags: Users,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/usersidorders-get-openapi.md
- name: Eventbrite Get Users Owned Event Orders
  x-api-slug: eventbrite
  description: |-
    Returns a paginated response of orders,
    under the key orders, of orders placed against any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/owned_event_orders/
  tags: Users,Owned,Event,Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/usersidowned-event-orders-get-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite brings people together through live experiences. Discover
    events that match your passions, or create your own with online ticketing tools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-crunchbase
  url: https://crunchbase.com/organization/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-twitter
  url: https://twitter.com/eventbrite
- type: x-website
  url: http://eventbriteapi.com
- type: x-website
  url: http://developer.eventbrite.com/
- type: x-website
  url: http://eventbrite.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---