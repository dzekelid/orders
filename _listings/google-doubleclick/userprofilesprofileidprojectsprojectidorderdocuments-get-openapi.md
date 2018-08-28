---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Order Documents
  version: 1.0.0
  description: Retrieves a list of order documents, possibly filtered. This method
    supports paging.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/projects/{projectId}/orders:
    get:
      summary: Get Orders
      description: Retrieves a list of orders, possibly filtered. This method supports
        paging.
      operationId: dfareporting.orders.list
      x-api-path-slug: userprofilesprofileidprojectsprojectidorders-get
      parameters:
      - in: query
        name: ids
        description: Select only orders with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for orders
      - in: query
        name: searchString
        description: Allows searching for orders by name or ID
      - in: query
        name: siteId
        description: Select only orders that are associated with these site IDs
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order
  /userprofiles/{profileId}/projects/{projectId}/orders/{id}:
    get:
      summary: Get Order
      description: Gets one order by ID.
      operationId: dfareporting.orders.get
      x-api-path-slug: userprofilesprofileidprojectsprojectidordersid-get
      parameters:
      - in: path
        name: id
        description: Order ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for orders
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order
  /userprofiles/{profileId}/projects/{projectId}/orderDocuments:
    get:
      summary: Get Order Documents
      description: Retrieves a list of order documents, possibly filtered. This method
        supports paging.
      operationId: dfareporting.orderDocuments.list
      x-api-path-slug: userprofilesprofileidprojectsprojectidorderdocuments-get
      parameters:
      - in: query
        name: approved
        description: Select only order documents that have been approved by at least
          one user
      - in: query
        name: ids
        description: Select only order documents with these IDs
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: orderId
        description: Select only order documents for specified orders
      - in: query
        name: pageToken
        description: Value of the nextPageToken from the previous result page
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      - in: query
        name: searchString
        description: Allows searching for order documents by name or ID
      - in: query
        name: siteId
        description: Select only order documents that are associated with these sites
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order Document
  /userprofiles/{profileId}/projects/{projectId}/orderDocuments/{id}:
    get:
      summary: Get Order Document
      description: Gets one order document by ID.
      operationId: dfareporting.orderDocuments.get
      x-api-path-slug: userprofilesprofileidprojectsprojectidorderdocumentsid-get
      parameters:
      - in: path
        name: id
        description: Order document ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: path
        name: projectId
        description: Project ID for order documents
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Order Document
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