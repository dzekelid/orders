---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Photosets Order Sets
  description: Set the order of photosets for the calling user.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---