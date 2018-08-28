---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List status histories of orders
  description: Lists the status histories of all orders. The result can be limited
    to an order, a status type, a period of time or a user.
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