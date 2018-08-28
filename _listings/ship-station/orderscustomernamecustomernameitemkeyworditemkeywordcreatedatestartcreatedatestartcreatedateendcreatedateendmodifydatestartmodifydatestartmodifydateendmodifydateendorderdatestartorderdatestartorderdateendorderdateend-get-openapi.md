---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station List Orders with parameters
  description: |-
    Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /orders?customerName={customerName}
    &itemKeyword={itemKeyword}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &modifyDateStart={modifyDateStart}
    &modifyDateEnd={modifyDateEnd}
    &orderDateStart={orderDateStart}
    &orderDateEnd={orderDateEnd}
    &orderNumber={orderNumber}
    &orderStatus={orderStatus}
    &paymentDateStart={paymentDateStart}
    &paymentDateEnd={paymentDateEnd}
    &storeId={storeId}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  version: 1.0.0
host: ssapi.shipstation.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders:
    get:
      summary: List Orders w/o parameters
      description: ""
      operationId: orders.get
      x-api-path-slug: orders-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - W
      - O
      - Parameters
  /orders/createorders:
    post:
      summary: Create/Update Multiple Orders
      description: |-
        This endpoint can be used to create or update multiple orders in one request. If the ``orderKey`` is specified in an order, the existing order with that key will be updated. Note: Only orders in an open status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``) can be updated through this method. ``cancelled`` and ``shipped`` are locked from modification through the API.

        Data Type          |Description
        -------------------|-------------------
        Order, required | An array of [**Order**](http://www.shipstation.com/developer-api/#/reference/model-order) objects (maximum of 100 per request)
      operationId: orders.createorders.post
      x-api-path-slug: orderscreateorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Orders
  /orders/listbytag?orderStatus={orderStatus}&tagId={tagId}&page={page}&pageSize={pageSize}:
    get:
      summary: List Orders by Tag
      description: |-
        Lists all orders that match the specified status and tag ID.

        Url format with filters:

        ```
        /listbytag?orderStatus={orderStatus}
        &tagId={tagId}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: orders.listbytag_orderStatus_orderStatus_tagId_tagId_page_page_pageSize_pageSize.get
      x-api-path-slug: orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get
      parameters:
      - in: path
        name: orderStatus
        description: The orders status
      - in: path
        name: page
        description: Page number
      - in: path
        name: pageSize
        description: Requested page size
      - in: path
        name: tagId
        description: ID of the tag
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Tag
  ? /orders?customerName={customerName}&itemKeyword={itemKeyword}&createDateStart={createDateStart}&createDateEnd={createDateEnd}&modifyDateStart={modifyDateStart}&modifyDateEnd={modifyDateEnd}&orderDateStart={orderDateStart}&orderDateEnd={orderDateEnd}&
  : get:
      summary: List Orders with parameters
      description: |-
        Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

        Url format with filters:

        ```
        /orders?customerName={customerName}
        &itemKeyword={itemKeyword}
        &createDateStart={createDateStart}
        &createDateEnd={createDateEnd}
        &modifyDateStart={modifyDateStart}
        &modifyDateEnd={modifyDateEnd}
        &orderDateStart={orderDateStart}
        &orderDateEnd={orderDateEnd}
        &orderNumber={orderNumber}
        &orderStatus={orderStatus}
        &paymentDateStart={paymentDateStart}
        &paymentDateEnd={paymentDateEnd}
        &storeId={storeId}
        &sortBy={sortBy}
        &sortDir={sortDir}
        &page={page}
        &pageSize={pageSize}
        ```
      operationId: orders_customerName_customerName_itemKeyword_itemKeyword_createDateStart_createDateStart_createDateE
      x-api-path-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
      parameters:
      - in: path
        name: createDateEnd
        description: Returns orders that were created in ShipStation before the specified
          date
      - in: path
        name: createDateStart
        description: Returns orders that were created in ShipStation after the specified
          date
      - in: path
        name: customerName
        description: Returns orders that match the specified name
      - in: path
        name: itemKeyword
        description: Returns orders that contain items that match the specified keyword
      - in: path
        name: modifyDateEnd
        description: Returns orders that were modified before the specified date
      - in: path
        name: modifyDateStart
        description: Returns orders that were modified after the specified date
      - in: path
        name: orderDateEnd
        description: Returns orders less than or equal to the specified date
      - in: path
        name: orderDateStart
        description: Returns orders greater than the specified date
      - in: path
        name: orderNumber
        description: Filter by order number, performs a starts with search
      - in: path
        name: orderStatus
        description: Filter by order status
      - in: path
        name: page
        description: Page number
      - in: path
        name: pageSize
        description: Requested page size
      - in: path
        name: paymentDateEnd
        description: Returns orders that were paid before the specified date
      - in: path
        name: paymentDateStart
        description: Returns orders that were paid after the specified date
      - in: path
        name: sortBy
        description: Sort the responses by a set value
      - in: path
        name: sortDir
        description: Sets the direction of the sort order
      - in: path
        name: storeId
        description: Filters orders to a single store
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - Parameters
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