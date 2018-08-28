swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/order/{playlistId}:
    post:
      summary: Order Widgets
      description: Set the order of widgets in the Playlist
      operationId: playlistOrder
      x-api-path-slug: playlistorderplaylistid-post
      parameters:
      - in: path
        name: playlistId
        description: The Playlist ID to Order
      - in: formData
        name: widgets
        description: Array of widgetIds and positions - all widgetIds present in the
          playlist need to be passed in the call with their positions
      responses:
        200:
          description: OK
      tags:
      - Order
      - Widgets