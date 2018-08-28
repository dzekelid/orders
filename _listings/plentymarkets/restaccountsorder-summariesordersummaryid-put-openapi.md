---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update an order summary
  description: Updates an order summary. The ID of the order summary must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders:
    get:
      summary: List orders by filter options
      description: List orders by filter options.
      operationId: getRestOrders
      x-api-path-slug: restorders-get
      parameters:
      - in: query
        name: clientId
        description: Filter that restricts the search result to order from one client
      - in: query
        name: contactId
        description: Filter that restricts the search result to orders of one order
          contact
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to orders that were created
          on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to orders that were created
          within a certain period of time
      - in: query
        name: externalOrderId
        description: Filter that restricts the search result to an external order
          id
      - in: query
        name: hasDocument
        description: Filter that restricts the search result to orders which hold
          the given document type
      - in: query
        name: includedItem
        description: Filter that restricts the search result to orders with a certain
          item
      - in: query
        name: includedVariation
        description: Filter that restricts the search result to orders with a certain
          variation
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to orders with ebay plus
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: orderIds
        description: Filter that restricts the search result to orders
      - in: query
        name: orderType
        description: Filter that restricts the search result to orders of specific
          order types
      - in: query
        name: outgoingItemsBookedAtFrom
        description: Filter that restricts the search result to orders where the outgoing
          items were booked on the specified date
      - in: query
        name: outgoingItemsBookedAtTo
        description: Filter that restricts the search result to orders where the outgoing
          items were booked within a specified period of time
      - in: query
        name: ownerUserId
        description: Filter that restricts the search result to orders of one owner
      - in: query
        name: page
        description: The page to get
      - in: query
        name: paidAtFrom
        description: Filter that restricts the search result to orders that received
          a payment on the specified date
      - in: query
        name: paidAtTo
        description: Filter that restricts the search result to orders that received
          a payment within a certain period of time
      - in: query
        name: paymentStatus
        description: Filter that restricts the search result to order with a specific
          payment status
      - in: query
        name: referrerId
        description: Filter that restricts the search result to orders from one order
          referrer
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to orders with a specific
          shipping profile
      - in: query
        name: statusFrom
        description: Filter that restricts the search result to orders in a specific
          order status
      - in: query
        name: statusTo
        description: Filter that restricts the search result to orders within a range
          of order statuses
      - in: query
        name: supplierId
        description: Filter that restricts the search result to orders that include
          order items with variations from a supplier
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to orders that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to orders that were last
          updated within a specified period of time
      - in: query
        name: warehouseId
        description: Filter that restricts the search result to orders with a specific
          main warehouse
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Filter
      - Options
    post:
      summary: Create an order
      description: Create an order.
      operationId: postRestOrders
      x-api-path-slug: restorders-post
      parameters:
      - in: body
        name: /rest/orders
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
  /rest/orders/contacts/{contactId}:
    get:
      summary: List orders of a contact
      description: Lists all orders of a contact. The ID of the contact must be specified.
      operationId: getRestOrdersContactsContact
      x-api-path-slug: restorderscontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - Of
      - Contact
  /rest/orders/status-history:
    get:
      summary: List status histories of orders
      description: Lists the status histories of all orders. The result can be limited
        to an order, a status type, a period of time or a user.
      operationId: getRestOrdersStatusHistory
      x-api-path-slug: restordersstatushistory-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: statusId
        description: The ID of the status
      - in: query
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Status
      - Histories
      - Of
      - Orders
  /rest/accounts/order_summaries:
    get:
      summary: List order summaries
      description: List order summaries.
      operationId: getRestAccountsOrderSummaries
      x-api-path-slug: restaccountsorder-summaries-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Summaries
    post:
      summary: Create an order summary
      description: Create an order summary.
      operationId: postRestAccountsOrderSummaries
      x-api-path-slug: restaccountsorder-summaries-post
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
  /rest/accounts/order_summaries/contacts/{contactId}:
    get:
      summary: Get an order summary by the contact ID
      description: Gets an order summary. The ID of the contact must be specified.
      operationId: getRestAccountsOrderSummariesContactsContact
      x-api-path-slug: restaccountsorder-summariescontactscontactid-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Contact
      - ID
  /rest/accounts/order_summaries/orders/{addressId}:
    get:
      summary: Get an order summary by the address ID
      description: Gets an order summary. The ID of the address must be specified.
      operationId: getRestAccountsOrderSummariesOrdersAddress
      x-api-path-slug: restaccountsorder-summariesordersaddressid-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Address
      - ID
  /rest/accounts/order_summaries/{orderSummaryId}:
    delete:
      summary: Delete an order summary
      description: Deletes an order summary. The ID of the order summary must be specified.
      operationId: deleteRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-delete
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
    get:
      summary: Get an order summary by the order summary ID
      description: Gets an order summary. The ID of the order summary must be specified.
      operationId: getRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-get
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
      - By
      - Order
      - Summary
      - ID
    put:
      summary: Update an order summary
      description: Updates an order summary. The ID of the order summary must be specified.
      operationId: putRestAccountsOrderSummariesOrdersummary
      x-api-path-slug: restaccountsorder-summariesordersummaryid-put
      parameters:
      - in: path
        name: orderSummaryId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Summary
  /rest/orders/addresses:
    post:
      summary: Create an address for existing order
      description: Creates an address for an existing order.
      operationId: postRestOrdersAddresses
      x-api-path-slug: restordersaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Addressexisting
      - Order
  /rest/orders/dates/types:
    get:
      summary: List order date types
      description: List order date types.
      operationId: getRestOrdersDatesTypes
      x-api-path-slug: restordersdatestypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Date
      - Types
  /rest/orders/dates/types/{typeId}:
    get:
      summary: Find an order date type by it's ID
      description: Find an order date type by it's id.
      operationId: getRestOrdersDatesTypesType
      x-api-path-slug: restordersdatestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Order
      - Date
      - Type
      - By
      - Its
      - ID
  /rest/orders/dates/types/{typeId}/names:
    get:
      summary: List names of an order date type
      description: Lists names in all languages available of an order date type. The
        ID of the date type must be specified.
      operationId: getRestOrdersDatesTypesTypeNames
      x-api-path-slug: restordersdatestypestypeidnames-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Order
      - Date
      - Type
  /rest/orders/dates/types/{typeId}/names/{lang}:
    get:
      summary: Get a name of an order date type
      description: Gets a name of an order date type. The ID of the date type and
        the language of the name must be specified.
      operationId: getRestOrdersDatesTypesTypeNamesLang
      x-api-path-slug: restordersdatestypestypeidnameslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Of
      - Order
      - Date
      - Type
  /rest/orders/items/dates:
    post:
      summary: Create a date for an order item
      description: Creates a date for an order item. The ID of the order item must
        be specified
      operationId: postRestOrdersItemsDates
      x-api-path-slug: restordersitemsdates-post
      parameters:
      - in: body
        name: /rest/orders/items/dates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
  /rest/orders/items/dates/{id}:
    delete:
      summary: Delete a date from an order item
      description: Deletes the date from an order item. The ID of the date must be
        specified.
      operationId: deleteRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
    get:
      summary: Get a date of an order item
      description: Gets a date of an order item. The ID of the date must be specified.
      operationId: getRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
    put:
      summary: Update a date of an order item
      description: Updates a date of an order item. The ID of the date must be specified.
      operationId: putRestOrdersItemsDates
      x-api-path-slug: restordersitemsdatesid-put
      parameters:
      - in: body
        name: /rest/orders/items/dates/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
  /rest/orders/items/properties:
    post:
      summary: Create an order item property.
      description: Create an order item property..
      operationId: postRestOrdersItemsProperties
      x-api-path-slug: restordersitemsproperties-post
      parameters:
      - in: body
        name: /rest/orders/items/properties
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
  /rest/orders/items/properties/{id}:
    delete:
      summary: Delete an order item property by ID.
      description: Delete an order item property by id..
      operationId: deleteRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    get:
      summary: Get an order item property by ID.
      description: Get an order item property by id..
      operationId: getRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
    put:
      summary: Update an order item property by ID.
      description: Update an order item property by id..
      operationId: putRestOrdersItemsProperties
      x-api-path-slug: restordersitemspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/items/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - ID
  /rest/orders/items/{orderItemId}/dates:
    get:
      summary: List dates of an order item
      description: Lists the dates of an order item. The ID of the order item must
        be specified.
      operationId: getRestOrdersItemsOrderitemDates
      x-api-path-slug: restordersitemsorderitemiddates-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
      - Item
  /rest/orders/items/{orderItemId}/dates/{typeId}:
    delete:
      summary: Delete a date from an order item by order item and date type
      description: Deletest a date from an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: deleteRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - From
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    get:
      summary: Get a date of an order item by order item and date type
      description: Gets a date of an order item. The ID of the order item and the
        ID of the date type must be specified.
      operationId: getRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    post:
      summary: Create a date for an order item by order item and date type
      description: Creates a date for an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: postRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Datean
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
    put:
      summary: Update a date of an order item by order item and date type
      description: Updates the date of an order item. The ID of the order item and
        the ID of the date type must be specified.
      operationId: putRestOrdersItemsOrderitemDatesType
      x-api-path-slug: restordersitemsorderitemiddatestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/dates/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Date
      - Of
      - Order
      - Item
      - By
      - Order
      - Item
      - Date
      - Type
  /rest/orders/items/{orderItemId}/properties:
    get:
      summary: Get all order item propertys for one order item by its order item id.
      description: Get all order item propertys for one order item by its order item
        id..
      operationId: getRestOrdersItemsOrderitemProperties
      x-api-path-slug: restordersitemsorderitemidproperties-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Propertysone
      - Order
      - Item
      - By
      - Its
      - Order
      - Item
      - Id
  /rest/orders/items/{orderItemId}/properties/{typeId}:
    delete:
      summary: Delete an order item property by order item ID and order property type
        ID.
      description: Delete an order item property by order item id and order property
        type id..
      operationId: deleteRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-delete
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    get:
      summary: Get an order item property by order item ID and order property type
        ID.
      description: Get an order item property by order item id and order property
        type id..
      operationId: getRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-get
      parameters:
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    post:
      summary: Create an order item property by order item ID and order property type
        ID.
      description: Create an order item property by order item id and order property
        type id..
      operationId: postRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-post
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
    put:
      summary: Update an order item property by order item ID and order property type
        ID.
      description: Update an order item property by order item id and order property
        type id..
      operationId: putRestOrdersItemsOrderitemPropertiesType
      x-api-path-slug: restordersitemsorderitemidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/items/{orderItemId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderItemId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
      - Property
      - By
      - Order
      - Item
      - ID
      - Order
      - Property
      - Type
      - ID
  /rest/orders/properties/types:
    get:
      summary: List order property types
      description: Lists property types and their names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Property
      - Types
    post:
      summary: Create an order property type
      description: Create an order property type.
      operationId: postRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-post
      parameters:
      - in: body
        name: /rest/orders/properties/types
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
      - Property
      - Type
  /rest/orders/properties/{id}:
    delete:
      summary: Delete a property of an order by property ID
      description: Deletes a property of an order. The ID of the property must be
        specified.
      operationId: deleteRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
    put:
      summary: Update a property of an order by property ID
      description: Updates the value of a property. The ID of the property must be
        specified.
      operationId: putRestOrdersProperties
      x-api-path-slug: restorderspropertiesid-put
      parameters:
      - in: body
        name: /rest/orders/properties/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Property
      - ID
  /rest/orders/referrers/{parentReferrerId?}:
    post:
      summary: Create an order referrer
      description: |-
        Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
        If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
        If the ID is automatically assigned, the first ID that has not been used before will be set.
        If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
      operationId: postRestOrdersReferrersParentreferrer
      x-api-path-slug: restordersreferrersparentreferrerid-post
      parameters:
      - in: query
        name: data
        description: The attributes of the order referrer to be created
      - in: path
        name: parentReferrerId?
      responses:
        200:
          description: OK
      tags:
      - Order
      - Referrer
  /rest/orders/shipping/export_documents/{orderId}:
    get:
      summary: List export documents by order ID
      description: List export documents by order id.
      operationId: getRestOrdersShippingExportDocumentsOrder
      x-api-path-slug: restordersshippingexport-documentsorderid-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Export
      - Documents
      - By
      - Order
      - ID
  /rest/orders/shipping/parcel_service_regions/{parcelServiceRegionId}:
    get:
      summary: Get an  order parcel service region
      description: Gets an parcel service region. The ID of the parcel service region
        must be specified.
      operationId: getRestOrdersShippingParcelServiceRegionsParcelserviceregion
      x-api-path-slug: restordersshippingparcel-service-regionsparcelserviceregionid-get
      parameters:
      - in: query
        name: $parcelServiceRegionId
        description: The ID of the parcel service region
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: parcelServiceRegionId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Parcel
      - Service
      - Region
  /rest/orders/statuses:
    get:
      summary: Searches order statuses.
      description: Searches for a list of order statuses, specified by the given filter
        parameters.
      operationId: getRestOrdersStatuses
      x-api-path-slug: restordersstatuses-get
      parameters:
      - in: query
        name: statusIdFrom
        description: Filter that restricts the search for order statuses to IDs from
          a defined value
      - in: query
        name: statusIdTo
        description: Filter that restricts the search for order statuses to IDs to
          a defined value
      responses:
        200:
          description: OK
      tags:
      - Searches
      - Order
      - Statuses
    post:
      summary: Creates an order status.
      description: Creates an order status, which is specified by the given ID.
      operationId: postRestOrdersStatuses
      x-api-path-slug: restordersstatuses-post
      parameters:
      - in: body
        name: /rest/orders/statuses
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Order
      - Status
  /rest/orders/statuses/{statusId}:
    delete:
      summary: Delete an order status.
      description: Deletes an order status, which is specified by the given ID.
      operationId: deleteRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-delete
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    get:
      summary: Get an order status.
      description: Gets an order status, which is specified by the given ID.
      operationId: getRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-get
      parameters:
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
    put:
      summary: Update an order status.
      description: Updates an order status, which is specified by the given ID.
      operationId: putRestOrdersStatusesStatus
      x-api-path-slug: restordersstatusesstatusid-put
      parameters:
      - in: body
        name: /rest/orders/statuses/{statusId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Status
  /rest/orders/{orderId}:
    delete:
      summary: Delete an order
      description: Deletes an order. The ID of the order must be specified.
      operationId: deleteRestOrdersOrder
      x-api-path-slug: restordersorderid-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
    get:
      summary: Get an order
      description: Gets an order. The ID of the order must be specified.
      operationId: getRestOrdersOrder
      x-api-path-slug: restordersorderid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - Order
    put:
      summary: Update an order
      description: Updates an order. The ID of the order must be specified.
      operationId: putRestOrdersOrder
      x-api-path-slug: restordersorderid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
  /rest/orders/{orderId}/addresses/{relationTypeId?}:
    get:
      summary: List order addresses
      description: Lists order addresses. The ID of the order must be specified.
      operationId: getRestOrdersOrderAddressesRelationtype
      x-api-path-slug: restordersorderidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: relationTypeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Addresses
  /rest/orders/{orderId}/cancel:
    put:
      summary: Cancel an order
      description: Cancels an order. The ID of the order must be specified.
      operationId: putRestOrdersOrderCancel
      x-api-path-slug: restordersorderidcancel-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/cancel
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Order
  /rest/orders/{orderId}/dates:
    get:
      summary: List dates of an order
      description: Lists dates of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderDates
      x-api-path-slug: restordersorderiddates-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
  /rest/orders/{orderId}/documents/downloads/{type?}:
    get:
      summary: Download documents of an order
      description: Downloads documents of an order as a zip file. The ID of the order
        must be specified. In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsDownloadsType
      x-api-path-slug: restordersorderiddocumentsdownloadstype-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the document
      - in: path
        name: type?
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type?}:
    get:
      summary: List documents of an order
      description: Lists documents of an order. The ID of the order must be specified.
        In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the order documents
      - in: path
        name: type?
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type}:
    post:
      summary: Upload order documents
      description: Uploads order documents. The ID of the order and the document type
        must be specified.
      operationId: postRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/documents/{type}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Order
      - Documents
  /rest/orders/{orderId}/items/serialNumbers:
    get:
      summary: List serial numbers of an order
      description: Lists all serial numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderItemsSerialnumbers
      x-api-path-slug: restordersorderiditemsserialnumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/items/{orderItemId}:
    delete:
      summary: Delete an order item
      description: Deletes an order item. The ID of the order and the ID of the order
        item must be specified.
      operationId: deleteRestOrdersOrderItemsOrderitem
      x-api-path-slug: restordersorderiditemsorderitemid-delete
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Item
  /rest/orders/{orderId}/items/{orderItemId}/serialNumbers:
    get:
      summary: List serial numbers of an order item
      description: Lists all serial numbers of an order item. The ID of the order
        and the ID of the order item must be specified.
      operationId: getRestOrdersOrderItemsOrderitemSerialnumbers
      x-api-path-slug: restordersorderiditemsorderitemidserialnumbers-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
      - Item
  /rest/orders/{orderId}/outgoing_stocks:
    post:
      summary: Book out order items
      description: Books out the order items of an order. The ID of the order must
        be specified and a booking date can be specified. The current date and time
        will be used if no date is specified.
      operationId: postRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-post
      parameters:
      - in: query
        name: date
        description: The date that is saved as booking date for the outgoing stock
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Out
      - Order
      - Items
  /rest/orders/{orderId}/packagenumbers:
    get:
      summary: List package numbers of an order
      description: Lists the package numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderPackagenumbers
      x-api-path-slug: restordersorderidpackagenumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Package
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/properties:
    post:
      summary: Create a property for an order
      description: Creates a property and attaches it to an order. The ID of the order
        must be specified.
      operationId: postRestOrdersOrderProperties
      x-api-path-slug: restordersorderidproperties-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Propertyan
      - Order
  /rest/orders/{orderId}/properties/{typeId?}:
    get:
      summary: List properties of an order
      description: Lists properties of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: typeId
        description: The property type ID
      - in: path
        name: typeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - Of
      - Order
  /rest/orders/{orderId}/properties/{typeId}:
    delete:
      summary: Delete a property of an order by order ID and type ID
      description: Deletes a property of an order. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: deleteRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-delete
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Type
      - ID
    put:
      summary: Update a property of an order by order ID and property ID
      description: Updates the value of a property. The composite key of the property
        must be specified. The composite key is composed of the ID of the order and
        the ID of the order property type.
      operationId: putRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/properties/{typeId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Property
      - Of
      - Order
      - By
      - Order
      - ID
      - Property
      - ID
  /rest/orders/{orderId}/shipping/packages:
    delete:
      summary: Delete all order shipping packages for an order
      description: Deletes all order shipping packages for an order. The ID of the
        order must be specified.
      operationId: deleteRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Packagesan
      - Order
    get:
      summary: List order shipping packages
      description: Lists order shipping packages. The ID of the order must be specified.
      operationId: getRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderId
      - in: query
        name: with
        description: Possible value is labelBase64
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Shipping
      - Packages
    post:
      summary: Create an order shipping package
      description: Creates an order shipping package. The ID of the order must be
        specified.
      operationId: postRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/shipping/packages
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
  /rest/orders/{orderId}/shipping/packages/{orderShippingPackageId}:
    delete:
      summary: Delete an order shipping package
      description: Deletes an order shipping package. The ID of the order and the
        ID of the order shipping package must be specified.
      operationId: deleteRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-delete
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
    get:
      summary: Get an order shipping package
      description: Gets an order shipping package. The ID of the order and the ID
        of the order shipping package must be specified.
      operationId: getRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
    put:
      summary: Update an order shipping package
      description: Updates an order shipping package. The ID of the order and the
        ID of the order shipping package must be specified.
      operationId: putRestOrdersOrderShippingPackagesOrdershippingpackage
      x-api-path-slug: restordersorderidshippingpackagesordershippingpackageid-put
      parameters:
      - in: body
        name: /rest/orders/{orderId}/shipping/packages/{orderShippingPackageId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: orderShippingPackageId
      responses:
        200:
          description: OK
      tags:
      - Order
      - Shipping
      - Package
  /rest/orders/{orderId}/status-history:
    get:
      summary: Get the status history of an order
      description: Gets the status of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderStatusHistory
      x-api-path-slug: restordersorderidstatushistory-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Status
      - History
      - Of
      - Order
  /rest/payments/orders/{orderId}:
    get:
      summary: List payments of an order
      description: Lists all payments of an order. The ID of the order must be specified.
      operationId: getRestPaymentsOrdersOrder
      x-api-path-slug: restpaymentsordersorderid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Order
  /rest/storage/order-properties/object-url:
    get:
      summary: Get the URL for a order property file
      description: |-
        Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
        minutes.
      operationId: getRestStorageOrderPropertiesObjectUrl
      x-api-path-slug: reststorageorderpropertiesobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the order property     *                        file
          to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Order
      - Property
      - File
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