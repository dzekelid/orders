swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/maps/{mapId}/orderlayers:
    post:
      summary: Update order of layers
      description: Updates the order of layers for a given map.
      operationId: updates-the-order-of-layers-for-a-given-map
      x-api-path-slug: v1mapsmapidorderlayers-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Order
      - Of
      - Layers