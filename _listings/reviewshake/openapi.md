swagger: "2.0"
x-collection-name: Reviewshake
x-complete: 1
info:
  title: Reviewshake API
  description: welcome-to-the-reviewshake-api-documentation-where-you-will-find-all-details-required-to-interact-with-our-api-in-order-to-make-calls-you-will-need-two-pieces-of-information1--your-reviewshake-subdomain-eg--demo-reviewshake-com2--your-api-key-see-the-authentication-section-below--authenticationyour-account-will-have-a-unique-api-key-associated-with-it-which-can-be-found-under--configurations----general-settings--in-your-dashboard-
  version: "1.0"
host: subdomain.reviewshake.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /order:
    post:
      summary: Create order
      description: |-
        Creating orders in Reviewshake allows you to automate the sending of review invitations. You can setup this automation in your dashboard by visiting *Review Invitations* -> *Triggers*.

        Set the *Trigger* as *Order created*, and you can then setup the trigger options such as templates and subject lines to use as well as delays.
      operationId: OrderPost
      x-api-path-slug: order-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: header
        name: X-Spree-Token
      responses:
        200:
          description: OK
      tags:
      - Order