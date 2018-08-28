---
name: Reviewshake
x-slug: reviewshake
description: Reviewshake helps you manage all your review sites from one place, automate
  new reviews from your customers and track review performance
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28931-subdomain-reviewshake-com.jpg
x-kinRank: "7"
x-alexaRank: ""
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reviewshake/apis.md
specificationVersion: "0.14"
apis:
- name: Reviewshake API - Create order
  x-api-slug: order-post
  description: |-
    Creating orders in Reviewshake allows you to automate the sending of review invitations. You can setup this automation in your dashboard by visiting *Review Invitations* -> *Triggers*.

    Set the *Trigger* as *Order created*, and you can then setup the trigger options such as templates and subject lines to use as well as delays.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28931-subdomain-reviewshake-com.jpg
  humanURL: https://www.reviewshake.com/
  baseURL: https://subdomain.reviewshake.com//api/v1
  tags: Reviews
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/reviewshake/order-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://request.baskets.api.gallery.streamdata.io
- type: x-twitter
  url: https://twitter.com/reviewshake
- type: x-website
  url: https://www.reviewshake.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---