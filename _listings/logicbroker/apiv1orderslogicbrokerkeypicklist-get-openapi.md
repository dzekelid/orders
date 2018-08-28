---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Get pick list for one order
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Orders/PickList:
    get:
      summary: Get pick lists for multiple orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetOrderPickListToken
      x-api-path-slug: apiv1orderspicklist-get
      parameters:
      - in: query
        name: FileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: query
        name: LogicbrokerKeys
        description: The logicbroker Keys
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Pick
      - Listsmultiple
      - Orders
  /api/v1/Orders:
    get:
      summary: Search orders
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_SearchSalesOrders
      x-api-path-slug: apiv1orders-get
      parameters:
      - in: query
        name: Filters.advanced
        description: Advanced query options
      - in: query
        name: Filters.from
        description: Beginning of time search window
      - in: query
        name: Filters.linkkey
        description: The linkkey identifies a group of related documents
      - in: query
        name: Filters.page
        description: Page number
      - in: query
        name: Filters.pageSize
        description: Page size
      - in: query
        name: Filters.partnerPO
        description: The partners purchase order number
      - in: query
        name: Filters.receiverCompanyId
        description: This Id is indicate who is received this document
      - in: query
        name: Filters.senderCompanyId
        description: This Id is indicate who is sent this document
      - in: query
        name: Filters.sourceKey
        description: Source key is usually the unique key the sender uses to find
          this document
      - in: query
        name: Filters.status
        description: The status of the document
      - in: query
        name: Filters.to
        description: End of time search window
      responses:
        200:
          description: OK
      tags:
      - Search
      - Orders
  /api/v1/Orders/CustomXML:
    post:
      summary: Create order(s) based on custom XML.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_UploadCustomXml
      x-api-path-slug: apiv1orderscustomxml-post
      parameters:
      - in: body
        name: data
        description: XML data to upload
        schema:
          $ref: '#/definitions/holder'
      - in: formData
        name: file
        description: File to upload
      - in: query
        name: xmlType
        description: XML type, leave blank unless directed otherwise
      responses:
        200:
          description: OK
      tags:
      - Order(s)
      - Based
      - "On"
      - Custom
      - XML
  /api/v1/Orders/{LogicbrokerKey}/Status/{Status}:
    put:
      summary: Update order status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_UpdateSalesOrderStatus
      x-api-path-slug: apiv1orderslogicbrokerkeystatusstatus-put
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      - in: path
        name: Status
        description: The Status
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
  /api/v1/Orders/{LogicbrokerKey}/Status:
    get:
      summary: Retrieve order status
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetSalesOrderStatus
      x-api-path-slug: apiv1orderslogicbrokerkeystatus-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Order
      - Status
  /api/v1/Orders/{LogicbrokerKey}:
    get:
      summary: Retrieve an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetSalesOrderDetails
      x-api-path-slug: apiv1orderslogicbrokerkey-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker Key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Order
  /api/v1/Orders/{LogicbrokerKey}/PickList:
    get:
      summary: Get pick list for one order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetOrderPickList
      x-api-path-slug: apiv1orderslogicbrokerkeypicklist-get
      parameters:
      - in: query
        name: FileType
        description: 'Valid types: jpg, png, pdf, ps, zpl'
      - in: path
        name: LogicbrokerKey
        description: The logicbroker Key
      - in: query
        name: ViewInBrowser
        description: Set to true to view the resulting link in the browser
      responses:
        200:
          description: OK
      tags:
      - Pick
      - Listone
      - Order
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