---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List orders by filter options
  x-api-slug: restorders-get
  description: List orders by filter options.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorders-get-openapi.md
- name: plentymarkets REST-API - List orders of a contact
  x-api-slug: restorderscontactscontactid-get
  description: Lists all orders of a contact. The ID of the contact must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderscontactscontactid-get-openapi.md
- name: plentymarkets REST-API - List status histories of orders
  x-api-slug: restordersstatushistory-get
  description: Lists the status histories of all orders. The result can be limited
    to an order, a status type, a period of time or a user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatushistory-get-openapi.md
- name: plentymarkets REST-API - List order summaries
  x-api-slug: restaccountsorder-summaries-get
  description: List order summaries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-openapi.md
- name: plentymarkets REST-API - Create an order summary
  x-api-slug: restaccountsorder-summaries-post
  description: Create an order summary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-openapi.md
- name: plentymarkets REST-API - Get an order summary by the contact ID
  x-api-slug: restaccountsorder-summariescontactscontactid-get
  description: Gets an order summary. The ID of the contact must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariescontactscontactid-get-openapi.md
- name: plentymarkets REST-API - Get an order summary by the address ID
  x-api-slug: restaccountsorder-summariesordersaddressid-get
  description: Gets an order summary. The ID of the address must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersaddressid-get-openapi.md
- name: plentymarkets REST-API - Delete an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-delete
  description: Deletes an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-openapi.md
- name: plentymarkets REST-API - Get an order summary by the order summary ID
  x-api-slug: restaccountsorder-summariesordersummaryid-get
  description: Gets an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-openapi.md
- name: plentymarkets REST-API - Update an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-put
  description: Updates an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-openapi.md
- name: plentymarkets REST-API - Create an order
  x-api-slug: restorders-post
  description: Create an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorders-post-openapi.md
- name: plentymarkets REST-API - Create an address for existing order
  x-api-slug: restordersaddresses-post
  description: Creates an address for an existing order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersaddresses-post-openapi.md
- name: plentymarkets REST-API - List order date types
  x-api-slug: restordersdatestypes-get
  description: List order date types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-openapi.md
- name: plentymarkets REST-API - Find an order date type by it's ID
  x-api-slug: restordersdatestypestypeid-get
  description: Find an order date type by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-openapi.md
- name: plentymarkets REST-API - List names of an order date type
  x-api-slug: restordersdatestypestypeidnames-get
  description: Lists names in all languages available of an order date type. The ID
    of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-openapi.md
- name: plentymarkets REST-API - Get a name of an order date type
  x-api-slug: restordersdatestypestypeidnameslang-get
  description: Gets a name of an order date type. The ID of the date type and the
    language of the name must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - List order property types
  x-api-slug: restorderspropertiestypes-get
  description: Lists property types and their names in all languages. Optionally one
    or more languages can be specified to get a limited response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-get-openapi.md
- name: plentymarkets REST-API - Create an order property type
  x-api-slug: restorderspropertiestypes-post
  description: Create an order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-post-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by property ID
  x-api-slug: restorderspropertiesid-delete
  description: Deletes a property of an order. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Update a property of an order by property ID
  x-api-slug: restorderspropertiesid-put
  description: Updates the value of a property. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-put-openapi.md
- name: plentymarkets REST-API - Create an order referrer
  x-api-slug: restordersreferrersparentreferrerid-post
  description: |-
    Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
    If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
    If the ID is automatically assigned, the first ID that has not been used before will be set.
    If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersreferrersparentreferrerid-post-openapi.md
- name: plentymarkets REST-API - List export documents by order ID
  x-api-slug: restordersshippingexport-documentsorderid-get
  description: List export documents by order id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingexport-documentsorderid-get-openapi.md
- name: plentymarkets REST-API - Get an  order parcel service region
  x-api-slug: restordersshippingparcel-service-regionsparcelserviceregionid-get
  description: Gets an parcel service region. The ID of the parcel service region
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingparcel-service-regionsparcelserviceregionid-get-openapi.md
- name: plentymarkets REST-API - Searches order statuses.
  x-api-slug: restordersstatuses-get
  description: Searches for a list of order statuses, specified by the given filter
    parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-get-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Delete an order
  x-api-slug: restordersorderid-delete
  description: Deletes an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-delete-openapi.md
- name: plentymarkets REST-API - Get an order
  x-api-slug: restordersorderid-get
  description: Gets an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-get-openapi.md
- name: plentymarkets REST-API - Update an order
  x-api-slug: restordersorderid-put
  description: Updates an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-put-openapi.md
- name: plentymarkets REST-API - List order addresses
  x-api-slug: restordersorderidaddressesrelationtypeid-get
  description: Lists order addresses. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-openapi.md
- name: plentymarkets REST-API - Cancel an order
  x-api-slug: restordersorderidcancel-put
  description: Cancels an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidcancel-put-openapi.md
- name: plentymarkets REST-API - List dates of an order
  x-api-slug: restordersorderiddates-get
  description: Lists dates of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-openapi.md
- name: plentymarkets REST-API - Download documents of an order
  x-api-slug: restordersorderiddocumentsdownloadstype-get
  description: Downloads documents of an order as a zip file. The ID of the order
    must be specified. In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List documents of an order
  x-api-slug: restordersorderiddocumentstype-get
  description: Lists documents of an order. The ID of the order must be specified.
    In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-get-openapi.md
- name: plentymarkets REST-API - Upload order documents
  x-api-slug: restordersorderiddocumentstype-post
  description: Uploads order documents. The ID of the order and the document type
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-post-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order
  x-api-slug: restordersorderiditemsserialnumbers-get
  description: Lists all serial numbers of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Book out order items
  x-api-slug: restordersorderidoutgoing-stocks-post
  description: Books out the order items of an order. The ID of the order must be
    specified and a booking date can be specified. The current date and time will
    be used if no date is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-post-openapi.md
- name: plentymarkets REST-API - List package numbers of an order
  x-api-slug: restordersorderidpackagenumbers-get
  description: Lists the package numbers of an order. The ID of the order must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-openapi.md
- name: plentymarkets REST-API - Create a property for an order
  x-api-slug: restordersorderidproperties-post
  description: Creates a property and attaches it to an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidproperties-post-openapi.md
- name: plentymarkets REST-API - List properties of an order
  x-api-slug: restordersorderidpropertiestypeid-get
  description: Lists properties of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by order ID and type
    ID
  x-api-slug: restordersorderidpropertiestypeid-delete
  description: Deletes a property of an order. The composite key of the property must
    be specified. The composite key is composed of the ID of the order and the ID
    of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Update a property of an order by order ID and property
    ID
  x-api-slug: restordersorderidpropertiestypeid-put
  description: Updates the value of a property. The composite key of the property
    must be specified. The composite key is composed of the ID of the order and the
    ID of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Delete all order shipping packages for an order
  x-api-slug: restordersorderidshippingpackages-delete
  description: Deletes all order shipping packages for an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-delete-openapi.md
- name: plentymarkets REST-API - List order shipping packages
  x-api-slug: restordersorderidshippingpackages-get
  description: Lists order shipping packages. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-openapi.md
- name: plentymarkets REST-API - Create an order shipping package
  x-api-slug: restordersorderidshippingpackages-post
  description: Creates an order shipping package. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-post-openapi.md
- name: plentymarkets REST-API - Delete an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-delete
  description: Deletes an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-delete-openapi.md
- name: plentymarkets REST-API - Get an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-get
  description: Gets an order shipping package. The ID of the order and the ID of the
    order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-get-openapi.md
- name: plentymarkets REST-API - Update an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-put
  description: Updates an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-put-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - List payments of an order
  x-api-slug: restpaymentsordersorderid-get
  description: Lists all payments of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restpaymentsordersorderid-get-openapi.md
- name: plentymarkets REST-API - Get the URL for a order property file
  x-api-slug: reststorageorderpropertiesobjecturl-get
  description: |-
    Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
    minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-openapi.md
- name: plentymarkets REST-API - List order summaries
  x-api-slug: restaccountsorder-summaries-get
  description: List order summaries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-openapi.md
- name: plentymarkets REST-API - Create an order summary
  x-api-slug: restaccountsorder-summaries-post
  description: Create an order summary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-openapi.md
- name: plentymarkets REST-API - Get an order summary by the contact ID
  x-api-slug: restaccountsorder-summariescontactscontactid-get
  description: Gets an order summary. The ID of the contact must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariescontactscontactid-get-openapi.md
- name: plentymarkets REST-API - Get an order summary by the address ID
  x-api-slug: restaccountsorder-summariesordersaddressid-get
  description: Gets an order summary. The ID of the address must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersaddressid-get-openapi.md
- name: plentymarkets REST-API - Delete an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-delete
  description: Deletes an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-openapi.md
- name: plentymarkets REST-API - Get an order summary by the order summary ID
  x-api-slug: restaccountsorder-summariesordersummaryid-get
  description: Gets an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-openapi.md
- name: plentymarkets REST-API - Update an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-put
  description: Updates an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-openapi.md
- name: plentymarkets REST-API - Create an order
  x-api-slug: restorders-post
  description: Create an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorders-post-openapi.md
- name: plentymarkets REST-API - Create an address for existing order
  x-api-slug: restordersaddresses-post
  description: Creates an address for an existing order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersaddresses-post-openapi.md
- name: plentymarkets REST-API - List order date types
  x-api-slug: restordersdatestypes-get
  description: List order date types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-openapi.md
- name: plentymarkets REST-API - Find an order date type by it's ID
  x-api-slug: restordersdatestypestypeid-get
  description: Find an order date type by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-openapi.md
- name: plentymarkets REST-API - List names of an order date type
  x-api-slug: restordersdatestypestypeidnames-get
  description: Lists names in all languages available of an order date type. The ID
    of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-openapi.md
- name: plentymarkets REST-API - Get a name of an order date type
  x-api-slug: restordersdatestypestypeidnameslang-get
  description: Gets a name of an order date type. The ID of the date type and the
    language of the name must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - List order property types
  x-api-slug: restorderspropertiestypes-get
  description: Lists property types and their names in all languages. Optionally one
    or more languages can be specified to get a limited response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-get-openapi.md
- name: plentymarkets REST-API - Create an order property type
  x-api-slug: restorderspropertiestypes-post
  description: Create an order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-post-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by property ID
  x-api-slug: restorderspropertiesid-delete
  description: Deletes a property of an order. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Update a property of an order by property ID
  x-api-slug: restorderspropertiesid-put
  description: Updates the value of a property. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-put-openapi.md
- name: plentymarkets REST-API - Create an order referrer
  x-api-slug: restordersreferrersparentreferrerid-post
  description: |-
    Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
    If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
    If the ID is automatically assigned, the first ID that has not been used before will be set.
    If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersreferrersparentreferrerid-post-openapi.md
- name: plentymarkets REST-API - List export documents by order ID
  x-api-slug: restordersshippingexport-documentsorderid-get
  description: List export documents by order id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingexport-documentsorderid-get-openapi.md
- name: plentymarkets REST-API - Get an  order parcel service region
  x-api-slug: restordersshippingparcel-service-regionsparcelserviceregionid-get
  description: Gets an parcel service region. The ID of the parcel service region
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingparcel-service-regionsparcelserviceregionid-get-openapi.md
- name: plentymarkets REST-API - Searches order statuses.
  x-api-slug: restordersstatuses-get
  description: Searches for a list of order statuses, specified by the given filter
    parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-get-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Delete an order
  x-api-slug: restordersorderid-delete
  description: Deletes an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-delete-openapi.md
- name: plentymarkets REST-API - Get an order
  x-api-slug: restordersorderid-get
  description: Gets an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-get-openapi.md
- name: plentymarkets REST-API - Update an order
  x-api-slug: restordersorderid-put
  description: Updates an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-put-openapi.md
- name: plentymarkets REST-API - List order addresses
  x-api-slug: restordersorderidaddressesrelationtypeid-get
  description: Lists order addresses. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-openapi.md
- name: plentymarkets REST-API - Cancel an order
  x-api-slug: restordersorderidcancel-put
  description: Cancels an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidcancel-put-openapi.md
- name: plentymarkets REST-API - List dates of an order
  x-api-slug: restordersorderiddates-get
  description: Lists dates of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-openapi.md
- name: plentymarkets REST-API - Download documents of an order
  x-api-slug: restordersorderiddocumentsdownloadstype-get
  description: Downloads documents of an order as a zip file. The ID of the order
    must be specified. In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List documents of an order
  x-api-slug: restordersorderiddocumentstype-get
  description: Lists documents of an order. The ID of the order must be specified.
    In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-get-openapi.md
- name: plentymarkets REST-API - Upload order documents
  x-api-slug: restordersorderiddocumentstype-post
  description: Uploads order documents. The ID of the order and the document type
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-post-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order
  x-api-slug: restordersorderiditemsserialnumbers-get
  description: Lists all serial numbers of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Book out order items
  x-api-slug: restordersorderidoutgoing-stocks-post
  description: Books out the order items of an order. The ID of the order must be
    specified and a booking date can be specified. The current date and time will
    be used if no date is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-post-openapi.md
- name: plentymarkets REST-API - List package numbers of an order
  x-api-slug: restordersorderidpackagenumbers-get
  description: Lists the package numbers of an order. The ID of the order must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-openapi.md
- name: plentymarkets REST-API - Create a property for an order
  x-api-slug: restordersorderidproperties-post
  description: Creates a property and attaches it to an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidproperties-post-openapi.md
- name: plentymarkets REST-API - List properties of an order
  x-api-slug: restordersorderidpropertiestypeid-get
  description: Lists properties of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by order ID and type
    ID
  x-api-slug: restordersorderidpropertiestypeid-delete
  description: Deletes a property of an order. The composite key of the property must
    be specified. The composite key is composed of the ID of the order and the ID
    of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Update a property of an order by order ID and property
    ID
  x-api-slug: restordersorderidpropertiestypeid-put
  description: Updates the value of a property. The composite key of the property
    must be specified. The composite key is composed of the ID of the order and the
    ID of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Delete all order shipping packages for an order
  x-api-slug: restordersorderidshippingpackages-delete
  description: Deletes all order shipping packages for an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-delete-openapi.md
- name: plentymarkets REST-API - List order shipping packages
  x-api-slug: restordersorderidshippingpackages-get
  description: Lists order shipping packages. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-openapi.md
- name: plentymarkets REST-API - Create an order shipping package
  x-api-slug: restordersorderidshippingpackages-post
  description: Creates an order shipping package. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-post-openapi.md
- name: plentymarkets REST-API - Delete an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-delete
  description: Deletes an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-delete-openapi.md
- name: plentymarkets REST-API - Get an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-get
  description: Gets an order shipping package. The ID of the order and the ID of the
    order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-get-openapi.md
- name: plentymarkets REST-API - Update an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-put
  description: Updates an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-put-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - List payments of an order
  x-api-slug: restpaymentsordersorderid-get
  description: Lists all payments of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restpaymentsordersorderid-get-openapi.md
- name: plentymarkets REST-API - Get the URL for a order property file
  x-api-slug: reststorageorderpropertiesobjecturl-get
  description: |-
    Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
    minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-openapi.md
- name: plentymarkets REST-API - Get the URL for a order property file
  x-api-slug: reststorageorderpropertiesobjecturl-get
  description: |-
    Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10
    minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/reststorageorderpropertiesobjecturl-get-openapi.md
- name: plentymarkets REST-API - List payments of an order
  x-api-slug: restpaymentsordersorderid-get
  description: Lists all payments of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restpaymentsordersorderid-get-openapi.md
- name: plentymarkets REST-API - Get the status history of an order
  x-api-slug: restordersorderidstatushistory-get
  description: Gets the status of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidstatushistory-get-openapi.md
- name: plentymarkets REST-API - Update an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-put
  description: Updates an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-put-openapi.md
- name: plentymarkets REST-API - Get an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-get
  description: Gets an order shipping package. The ID of the order and the ID of the
    order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-get-openapi.md
- name: plentymarkets REST-API - Delete an order shipping package
  x-api-slug: restordersorderidshippingpackagesordershippingpackageid-delete
  description: Deletes an order shipping package. The ID of the order and the ID of
    the order shipping package must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackagesordershippingpackageid-delete-openapi.md
- name: plentymarkets REST-API - Create an order shipping package
  x-api-slug: restordersorderidshippingpackages-post
  description: Creates an order shipping package. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-post-openapi.md
- name: plentymarkets REST-API - List order shipping packages
  x-api-slug: restordersorderidshippingpackages-get
  description: Lists order shipping packages. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-get-openapi.md
- name: plentymarkets REST-API - Delete all order shipping packages for an order
  x-api-slug: restordersorderidshippingpackages-delete
  description: Deletes all order shipping packages for an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidshippingpackages-delete-openapi.md
- name: plentymarkets REST-API - Update a property of an order by order ID and property
    ID
  x-api-slug: restordersorderidpropertiestypeid-put
  description: Updates the value of a property. The composite key of the property
    must be specified. The composite key is composed of the ID of the order and the
    ID of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by order ID and type
    ID
  x-api-slug: restordersorderidpropertiestypeid-delete
  description: Deletes a property of an order. The composite key of the property must
    be specified. The composite key is composed of the ID of the order and the ID
    of the order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - List properties of an order
  x-api-slug: restordersorderidpropertiestypeid-get
  description: Lists properties of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Create a property for an order
  x-api-slug: restordersorderidproperties-post
  description: Creates a property and attaches it to an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidproperties-post-openapi.md
- name: plentymarkets REST-API - List package numbers of an order
  x-api-slug: restordersorderidpackagenumbers-get
  description: Lists the package numbers of an order. The ID of the order must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidpackagenumbers-get-openapi.md
- name: plentymarkets REST-API - Book out order items
  x-api-slug: restordersorderidoutgoing-stocks-post
  description: Books out the order items of an order. The ID of the order must be
    specified and a booking date can be specified. The current date and time will
    be used if no date is specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-post-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order item
  x-api-slug: restordersorderiditemsorderitemidserialnumbers-get
  description: Lists all serial numbers of an order item. The ID of the order and
    the ID of the order item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemidserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Delete an order item
  x-api-slug: restordersorderiditemsorderitemid-delete
  description: Deletes an order item. The ID of the order and the ID of the order
    item must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsorderitemid-delete-openapi.md
- name: plentymarkets REST-API - List serial numbers of an order
  x-api-slug: restordersorderiditemsserialnumbers-get
  description: Lists all serial numbers of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiditemsserialnumbers-get-openapi.md
- name: plentymarkets REST-API - Upload order documents
  x-api-slug: restordersorderiddocumentstype-post
  description: Uploads order documents. The ID of the order and the document type
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-post-openapi.md
- name: plentymarkets REST-API - List documents of an order
  x-api-slug: restordersorderiddocumentstype-get
  description: Lists documents of an order. The ID of the order must be specified.
    In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentstype-get-openapi.md
- name: plentymarkets REST-API - Download documents of an order
  x-api-slug: restordersorderiddocumentsdownloadstype-get
  description: Downloads documents of an order as a zip file. The ID of the order
    must be specified. In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List dates of an order
  x-api-slug: restordersorderiddates-get
  description: Lists dates of an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderiddates-get-openapi.md
- name: plentymarkets REST-API - Cancel an order
  x-api-slug: restordersorderidcancel-put
  description: Cancels an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidcancel-put-openapi.md
- name: plentymarkets REST-API - List order addresses
  x-api-slug: restordersorderidaddressesrelationtypeid-get
  description: Lists order addresses. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderidaddressesrelationtypeid-get-openapi.md
- name: plentymarkets REST-API - Update an order
  x-api-slug: restordersorderid-put
  description: Updates an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-put-openapi.md
- name: plentymarkets REST-API - Get an order
  x-api-slug: restordersorderid-get
  description: Gets an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-get-openapi.md
- name: plentymarkets REST-API - Delete an order
  x-api-slug: restordersorderid-delete
  description: Deletes an order. The ID of the order must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersorderid-delete-openapi.md
- name: plentymarkets REST-API - Update an order status.
  x-api-slug: restordersstatusesstatusid-put
  description: Updates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-put-openapi.md
- name: plentymarkets REST-API - Get an order status.
  x-api-slug: restordersstatusesstatusid-get
  description: Gets an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-get-openapi.md
- name: plentymarkets REST-API - Delete an order status.
  x-api-slug: restordersstatusesstatusid-delete
  description: Deletes an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatusesstatusid-delete-openapi.md
- name: plentymarkets REST-API - Creates an order status.
  x-api-slug: restordersstatuses-post
  description: Creates an order status, which is specified by the given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-post-openapi.md
- name: plentymarkets REST-API - Searches order statuses.
  x-api-slug: restordersstatuses-get
  description: Searches for a list of order statuses, specified by the given filter
    parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersstatuses-get-openapi.md
- name: plentymarkets REST-API - Get an  order parcel service region
  x-api-slug: restordersshippingparcel-service-regionsparcelserviceregionid-get
  description: Gets an parcel service region. The ID of the parcel service region
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingparcel-service-regionsparcelserviceregionid-get-openapi.md
- name: plentymarkets REST-API - List export documents by order ID
  x-api-slug: restordersshippingexport-documentsorderid-get
  description: List export documents by order id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersshippingexport-documentsorderid-get-openapi.md
- name: plentymarkets REST-API - Create an order referrer
  x-api-slug: restordersreferrersparentreferrerid-post
  description: |-
    Create an order referrer. The ID can be specified, a parent ID can be specified to create a sub referrer or if no ID is specified, a referrer ID will be assigned automatically.
    If an ID is specified, the ID may not be used already. If the ID is used already, the referrer will only be created.
    If the ID is automatically assigned, the first ID that has not been used before will be set.
    If the ID is not specified, but a parent referrer ID is given, then the new referrer ID will be a sub referrer of the given parent.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersreferrersparentreferrerid-post-openapi.md
- name: plentymarkets REST-API - Update a property of an order by property ID
  x-api-slug: restorderspropertiesid-put
  description: Updates the value of a property. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-put-openapi.md
- name: plentymarkets REST-API - Delete a property of an order by property ID
  x-api-slug: restorderspropertiesid-delete
  description: Deletes a property of an order. The ID of the property must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Create an order property type
  x-api-slug: restorderspropertiestypes-post
  description: Create an order property type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-post-openapi.md
- name: plentymarkets REST-API - List order property types
  x-api-slug: restorderspropertiestypes-get
  description: Lists property types and their names in all languages. Optionally one
    or more languages can be specified to get a limited response.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorderspropertiestypes-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-put
  description: Update an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-put-openapi.md
- name: plentymarkets REST-API - Create an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-post
  description: Create an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-post-openapi.md
- name: plentymarkets REST-API - Get an order item property by order item ID and order
    property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-get
  description: Get an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by order item ID and
    order property type ID.
  x-api-slug: restordersitemsorderitemidpropertiestypeid-delete
  description: Delete an order item property by order item id and order property type
    id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidpropertiestypeid-delete-openapi.md
- name: plentymarkets REST-API - Get all order item propertys for one order item by
    its order item id.
  x-api-slug: restordersitemsorderitemidproperties-get
  description: Get all order item propertys for one order item by its order item id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemidproperties-get-openapi.md
- name: plentymarkets REST-API - Update a date of an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-put
  description: Updates the date of an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-put-openapi.md
- name: plentymarkets REST-API - Create a date for an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-post
  description: Creates a date for an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-post-openapi.md
- name: plentymarkets REST-API - Get a date of an order item by order item and date
    type
  x-api-slug: restordersitemsorderitemiddatestypeid-get
  description: Gets a date of an order item. The ID of the order item and the ID of
    the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item by order item and
    date type
  x-api-slug: restordersitemsorderitemiddatestypeid-delete
  description: Deletest a date from an order item. The ID of the order item and the
    ID of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddatestypeid-delete-openapi.md
- name: plentymarkets REST-API - List dates of an order item
  x-api-slug: restordersitemsorderitemiddates-get
  description: Lists the dates of an order item. The ID of the order item must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsorderitemiddates-get-openapi.md
- name: plentymarkets REST-API - Update an order item property by ID.
  x-api-slug: restordersitemspropertiesid-put
  description: Update an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-put-openapi.md
- name: plentymarkets REST-API - Get an order item property by ID.
  x-api-slug: restordersitemspropertiesid-get
  description: Get an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-get-openapi.md
- name: plentymarkets REST-API - Delete an order item property by ID.
  x-api-slug: restordersitemspropertiesid-delete
  description: Delete an order item property by id..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemspropertiesid-delete-openapi.md
- name: plentymarkets REST-API - Create an order item property.
  x-api-slug: restordersitemsproperties-post
  description: Create an order item property..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsproperties-post-openapi.md
- name: plentymarkets REST-API - Update a date of an order item
  x-api-slug: restordersitemsdatesid-put
  description: Updates a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-put-openapi.md
- name: plentymarkets REST-API - Get a date of an order item
  x-api-slug: restordersitemsdatesid-get
  description: Gets a date of an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-get-openapi.md
- name: plentymarkets REST-API - Delete a date from an order item
  x-api-slug: restordersitemsdatesid-delete
  description: Deletes the date from an order item. The ID of the date must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdatesid-delete-openapi.md
- name: plentymarkets REST-API - Create a date for an order item
  x-api-slug: restordersitemsdates-post
  description: Creates a date for an order item. The ID of the order item must be
    specified
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersitemsdates-post-openapi.md
- name: plentymarkets REST-API - Get a name of an order date type
  x-api-slug: restordersdatestypestypeidnameslang-get
  description: Gets a name of an order date type. The ID of the date type and the
    language of the name must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnameslang-get-openapi.md
- name: plentymarkets REST-API - List names of an order date type
  x-api-slug: restordersdatestypestypeidnames-get
  description: Lists names in all languages available of an order date type. The ID
    of the date type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeidnames-get-openapi.md
- name: plentymarkets REST-API - Find an order date type by it's ID
  x-api-slug: restordersdatestypestypeid-get
  description: Find an order date type by it's id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypestypeid-get-openapi.md
- name: plentymarkets REST-API - List order date types
  x-api-slug: restordersdatestypes-get
  description: List order date types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersdatestypes-get-openapi.md
- name: plentymarkets REST-API - Create an address for existing order
  x-api-slug: restordersaddresses-post
  description: Creates an address for an existing order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restordersaddresses-post-openapi.md
- name: plentymarkets REST-API - Create an order
  x-api-slug: restorders-post
  description: Create an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restorders-post-openapi.md
- name: plentymarkets REST-API - Update an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-put
  description: Updates an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-put-openapi.md
- name: plentymarkets REST-API - Get an order summary by the order summary ID
  x-api-slug: restaccountsorder-summariesordersummaryid-get
  description: Gets an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-get-openapi.md
- name: plentymarkets REST-API - Delete an order summary
  x-api-slug: restaccountsorder-summariesordersummaryid-delete
  description: Deletes an order summary. The ID of the order summary must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersummaryid-delete-openapi.md
- name: plentymarkets REST-API - Get an order summary by the address ID
  x-api-slug: restaccountsorder-summariesordersaddressid-get
  description: Gets an order summary. The ID of the address must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariesordersaddressid-get-openapi.md
- name: plentymarkets REST-API - Get an order summary by the contact ID
  x-api-slug: restaccountsorder-summariescontactscontactid-get
  description: Gets an order summary. The ID of the contact must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summariescontactscontactid-get-openapi.md
- name: plentymarkets REST-API - Create an order summary
  x-api-slug: restaccountsorder-summaries-post
  description: Create an order summary.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-post-openapi.md
- name: plentymarkets REST-API - List order summaries
  x-api-slug: restaccountsorder-summaries-get
  description: List order summaries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/plentymarkets/restaccountsorder-summaries-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---