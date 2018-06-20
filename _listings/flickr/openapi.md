---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.photosets.orderSets:
    post:
      summary: Photosets Order Sets
      description: Set the order of photosets for the calling user.
      operationId: postRestMethodFlickr.photosets.ordersets
      x-api-path-slug: restmethodflickr-photosets-ordersets-post
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: photoset_ids
        description: A comma delimited list of photoset IDs, ordered with the set
          to show first, first in the list
      responses:
        200:
          description: OK
      tags:
      - Photosets
      - OrderSets
---