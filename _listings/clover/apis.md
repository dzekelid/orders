---
name: Clover
x-slug: clover
description: Clover, a First Data company, builds the largest open-architecture point
  of sale solution aimed at small &amp; medium sized business owners. Our products
  are changing the consumer/merchant experience for the better, opening avenues for
  seamless customer-merchant interactions. There are five versions of Clover, including
  the Clover Station, Clover Mobile, Clover Mini, Clover Go, and Clover Flex. With
  Clover, First Data is aiming to create the largest open architecture operating system
  for commerce-enabling solutions and applications for business owners.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
x-kinRank: "7"
x-alexaRank: "23096"
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/apis.md
specificationVersion: "0.14"
apis:
- name: ' - Gets a list of orders'
  x-api-slug: v3merchantsmidorders-get
  description: Returns a list of orders. See https://docs.clover.com/build/working-with-orders/
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorders-get-openapi.md
- name: ' - Get all orders for an employee'
  x-api-slug: v3merchantsmidemployeesempidorders-get
  description: Get all orders for an employee.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidemployeesempidorders-get-openapi.md
- name: ' - Create an order'
  x-api-slug: v3merchantsmidorders-post
  description: Only supports basic order creation. Valid fields are limited to taxRemoved,
    note, title, and orderType. Adding line items must be done in separate calls.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorders-post-openapi.md
- name: ' - Get a single order'
  x-api-slug: v3merchantsmidordersorderid-get
  description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-get-openapi.md
- name: ' - Update an order'
  x-api-slug: v3merchantsmidordersorderid-post
  description: Update an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-post-openapi.md
- name: ' - Delete an order'
  x-api-slug: v3merchantsmidordersorderid-delete
  description: Delete an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-delete-openapi.md
- name: ' - Get all discounts for an order'
  x-api-slug: v3merchantsmidordersorderiddiscounts-get
  description: Get all discounts for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-get-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscountsdiscountid-delete-openapi.md
- name: ' - Get all line items for an order'
  x-api-slug: v3merchantsmidordersorderidline-items-get
  description: Get all line items for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-get-openapi.md
- name: ' - Create a new line item'
  x-api-slug: v3merchantsmidordersorderidline-items-post
  description: Create a new line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-post-openapi.md
- name: ' - Get a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-get
  description: Get a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-get-openapi.md
- name: ' - Update a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-post
  description: Update a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-post-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-delete-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete-openapi.md
- name: ' - Apply a modification to a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
  description: 'Create a modification, a record of a modifier as it exists at the
    time it is applied to the lineItem. To view current modifications use an ''expand=modifications''
    query parameter on the lineItem. To learn more about applying a modification see:
    https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodifications-post-openapi.md
- name: ' - Remove a modification from a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
  description: Delete a modification by UUID, removing the record of an applied modification
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete-openapi.md
- name: ' - Create multiple line items in bulk.'
  x-api-slug: v3merchantsmidordersorderidbulk-line-items-post
  description: Create multiple line items in bulk..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidbulk-line-items-post-openapi.md
- name: ' - Create a payment record on an order'
  x-api-slug: v3merchantsmidordersorderidpayments-post
  description: Create a payment record on an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-post-openapi.md
- name: ' - Update the priorities for a collection of up to 200 modifier groups at
    a time'
  x-api-slug: v3merchantsmidmodifier-group-sort-orders-post
  description: Update the priorities for a collection of up to 200 modifier groups
    at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidmodifier-group-sort-orders-post-openapi.md
- name: ' - Get all payments for an order'
  x-api-slug: v3merchantsmidordersorderidpayments-get
  description: Get all payments for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-get-openapi.md
- name: ' - '
  x-api-slug: v3merchantsmidordersorderidservice-charge-post
  description: .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-charge-post-openapi.md
- name: ' - Remove service charge from an order'
  x-api-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
  description: Remove service charge from an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-chargechargeid-delete-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidvoided-line-items-post
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidvoided-line-items-post-openapi.md
- name: ' - Create or exchange a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
  description: Create or exchange a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post-openapi.md
- name: ' - Get all order types for a merchant'
  x-api-slug: v3merchantsmidorder-types-get
  description: Merchants have the ability to create custom order types via the Setup
    App (https://www.clover.com/setupapp). These custom order types can be associated
    with a System Order Type (see /v3/merchants/{mId}/system_order_types). Custom
    Order Types can support items in all categories (filterCategories=false) or a
    subset of the merchant's categories (filterCategories=true and categories property
    contains the list of supported categories). Note that when expanding the categories
    for an order type, they will only be returned if this orderType only supports
    a subset of the categories (filterCategories=true). If the orderType supports
    all categories (filterCategories=false) then you should make a GET request to
    /v3/merchants/{mId}/categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-get-openapi.md
- name: ' - Create Order Type For Merchant'
  x-api-slug: v3merchantsmidorder-types-post
  description: Create order type for merchant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Create or delete a order type category'
  x-api-slug: v3merchantsmidorder-type-categories-post
  description: Create or delete a order type category.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-type-categories-post-openapi.md
- name: ' - Return a list of system order types'
  x-api-slug: v3merchantsmidsystem-order-types-get
  description: Merchants can create custom Order Types via "/v3/merchants/{mId}/order_types".
    It is useful to associate these custom order types with particular system order
    types in order to group things functionally. For example, a merchant may have
    a "Lunch Take-Out" order type and a "Dinner Take-Out" order type. These two order
    types can be associated with the "TAKE-OUT-TYPE" system order type so that applications
    can understand that they are both take-out order types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidsystem-order-types-get-openapi.md
- name: ' - Get a single order'
  x-api-slug: v3merchantsmidordersorderid-get
  description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-get-openapi.md
- name: ' - Update an order'
  x-api-slug: v3merchantsmidordersorderid-post
  description: Update an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-post-openapi.md
- name: ' - Delete an order'
  x-api-slug: v3merchantsmidordersorderid-delete
  description: Delete an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-delete-openapi.md
- name: ' - Get all discounts for an order'
  x-api-slug: v3merchantsmidordersorderiddiscounts-get
  description: Get all discounts for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-get-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscountsdiscountid-delete-openapi.md
- name: ' - Get all line items for an order'
  x-api-slug: v3merchantsmidordersorderidline-items-get
  description: Get all line items for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-get-openapi.md
- name: ' - Create a new line item'
  x-api-slug: v3merchantsmidordersorderidline-items-post
  description: Create a new line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-post-openapi.md
- name: ' - Get a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-get
  description: Get a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-get-openapi.md
- name: ' - Update a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-post
  description: Update a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-post-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-delete-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete-openapi.md
- name: ' - Apply a modification to a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
  description: 'Create a modification, a record of a modifier as it exists at the
    time it is applied to the lineItem. To view current modifications use an ''expand=modifications''
    query parameter on the lineItem. To learn more about applying a modification see:
    https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodifications-post-openapi.md
- name: ' - Remove a modification from a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
  description: Delete a modification by UUID, removing the record of an applied modification
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete-openapi.md
- name: ' - Create multiple line items in bulk.'
  x-api-slug: v3merchantsmidordersorderidbulk-line-items-post
  description: Create multiple line items in bulk..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidbulk-line-items-post-openapi.md
- name: ' - Create a payment record on an order'
  x-api-slug: v3merchantsmidordersorderidpayments-post
  description: Create a payment record on an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-post-openapi.md
- name: ' - Get all payments for an order'
  x-api-slug: v3merchantsmidordersorderidpayments-get
  description: Get all payments for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-get-openapi.md
- name: ' - '
  x-api-slug: v3merchantsmidordersorderidservice-charge-post
  description: .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-charge-post-openapi.md
- name: ' - Remove service charge from an order'
  x-api-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
  description: Remove service charge from an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-chargechargeid-delete-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidvoided-line-items-post
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidvoided-line-items-post-openapi.md
- name: ' - Create or exchange a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
  description: Create or exchange a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Get all order types for a merchant'
  x-api-slug: v3merchantsmidorder-types-get
  description: Merchants have the ability to create custom order types via the Setup
    App (https://www.clover.com/setupapp). These custom order types can be associated
    with a System Order Type (see /v3/merchants/{mId}/system_order_types). Custom
    Order Types can support items in all categories (filterCategories=false) or a
    subset of the merchant's categories (filterCategories=true and categories property
    contains the list of supported categories). Note that when expanding the categories
    for an order type, they will only be returned if this orderType only supports
    a subset of the categories (filterCategories=true). If the orderType supports
    all categories (filterCategories=false) then you should make a GET request to
    /v3/merchants/{mId}/categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-get-openapi.md
- name: ' - Create Order Type For Merchant'
  x-api-slug: v3merchantsmidorder-types-post
  description: Create order type for merchant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Create or delete a order type category'
  x-api-slug: v3merchantsmidorder-type-categories-post
  description: Create or delete a order type category.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-type-categories-post-openapi.md
- name: ' - Return a list of system order types'
  x-api-slug: v3merchantsmidsystem-order-types-get
  description: Merchants can create custom Order Types via "/v3/merchants/{mId}/order_types".
    It is useful to associate these custom order types with particular system order
    types in order to group things functionally. For example, a merchant may have
    a "Lunch Take-Out" order type and a "Dinner Take-Out" order type. These two order
    types can be associated with the "TAKE-OUT-TYPE" system order type so that applications
    can understand that they are both take-out order types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidsystem-order-types-get-openapi.md
- name: ' - Get a single order'
  x-api-slug: v3merchantsmidordersorderid-get
  description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-get-openapi.md
- name: ' - Update an order'
  x-api-slug: v3merchantsmidordersorderid-post
  description: Update an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-post-openapi.md
- name: ' - Delete an order'
  x-api-slug: v3merchantsmidordersorderid-delete
  description: Delete an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-delete-openapi.md
- name: ' - Get all discounts for an order'
  x-api-slug: v3merchantsmidordersorderiddiscounts-get
  description: Get all discounts for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-get-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscountsdiscountid-delete-openapi.md
- name: ' - Get all line items for an order'
  x-api-slug: v3merchantsmidordersorderidline-items-get
  description: Get all line items for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-get-openapi.md
- name: ' - Create a new line item'
  x-api-slug: v3merchantsmidordersorderidline-items-post
  description: Create a new line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-post-openapi.md
- name: ' - Get a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-get
  description: Get a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-get-openapi.md
- name: ' - Update a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-post
  description: Update a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-post-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-delete-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscounts-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete-openapi.md
- name: ' - Apply a modification to a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
  description: 'Create a modification, a record of a modifier as it exists at the
    time it is applied to the lineItem. To view current modifications use an ''expand=modifications''
    query parameter on the lineItem. To learn more about applying a modification see:
    https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodifications-post-openapi.md
- name: ' - Remove a modification from a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
  description: Delete a modification by UUID, removing the record of an applied modification
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete-openapi.md
- name: ' - Create multiple line items in bulk.'
  x-api-slug: v3merchantsmidordersorderidbulk-line-items-post
  description: Create multiple line items in bulk..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidbulk-line-items-post-openapi.md
- name: ' - Create a payment record on an order'
  x-api-slug: v3merchantsmidordersorderidpayments-post
  description: Create a payment record on an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-post-openapi.md
- name: ' - Get all payments for an order'
  x-api-slug: v3merchantsmidordersorderidpayments-get
  description: Get all payments for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-get-openapi.md
- name: ' - '
  x-api-slug: v3merchantsmidordersorderidservice-charge-post
  description: .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-charge-post-openapi.md
- name: ' - Remove service charge from an order'
  x-api-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
  description: Remove service charge from an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-chargechargeid-delete-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidvoided-line-items-post
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidvoided-line-items-post-openapi.md
- name: ' - Create or exchange a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
  description: Create or exchange a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Return a list of system order types'
  x-api-slug: v3merchantsmidsystem-order-types-get
  description: Merchants can create custom Order Types via "/v3/merchants/{mId}/order_types".
    It is useful to associate these custom order types with particular system order
    types in order to group things functionally. For example, a merchant may have
    a "Lunch Take-Out" order type and a "Dinner Take-Out" order type. These two order
    types can be associated with the "TAKE-OUT-TYPE" system order type so that applications
    can understand that they are both take-out order types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidsystem-order-types-get-openapi.md
- name: ' - Create or delete a order type category'
  x-api-slug: v3merchantsmidorder-type-categories-post
  description: Create or delete a order type category.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-type-categories-post-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
- name: ' - Create Order Type For Merchant'
  x-api-slug: v3merchantsmidorder-types-post
  description: Create order type for merchant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-post-openapi.md
- name: ' - Get all order types for a merchant'
  x-api-slug: v3merchantsmidorder-types-get
  description: Merchants have the ability to create custom order types via the Setup
    App (https://www.clover.com/setupapp). These custom order types can be associated
    with a System Order Type (see /v3/merchants/{mId}/system_order_types). Custom
    Order Types can support items in all categories (filterCategories=false) or a
    subset of the merchant's categories (filterCategories=true and categories property
    contains the list of supported categories). Note that when expanding the categories
    for an order type, they will only be returned if this orderType only supports
    a subset of the categories (filterCategories=true). If the orderType supports
    all categories (filterCategories=false) then you should make a GET request to
    /v3/merchants/{mId}/categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-types-get-openapi.md
- name: ' - Create or exchange a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
  description: Create or exchange a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidvoided-line-items-post
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidvoided-line-items-post-openapi.md
- name: ' - Remove service charge from an order'
  x-api-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
  description: Remove service charge from an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-chargechargeid-delete-openapi.md
- name: ' - '
  x-api-slug: v3merchantsmidordersorderidservice-charge-post
  description: .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidservice-charge-post-openapi.md
- name: ' - Get all payments for an order'
  x-api-slug: v3merchantsmidordersorderidpayments-get
  description: Get all payments for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-get-openapi.md
- name: ' - Create a payment record on an order'
  x-api-slug: v3merchantsmidordersorderidpayments-post
  description: Create a payment record on an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidpayments-post-openapi.md
- name: ' - Create multiple line items in bulk.'
  x-api-slug: v3merchantsmidordersorderidbulk-line-items-post
  description: Create multiple line items in bulk..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidbulk-line-items-post-openapi.md
- name: ' - Remove a modification from a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
  description: Delete a modification by UUID, removing the record of an applied modification
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete-openapi.md
- name: ' - Apply a modification to a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
  description: 'Create a modification, a record of a modifier as it exists at the
    time it is applied to the lineItem. To view current modifications use an ''expand=modifications''
    query parameter on the lineItem. To learn more about applying a modification see:
    https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodifications-post-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemiddiscounts-post-openapi.md
- name: ' - Void a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
  description: Void a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-delete-openapi.md
- name: ' - Update a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-post
  description: Update a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-post-openapi.md
- name: ' - Get a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemid-get
  description: Get a line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemid-get-openapi.md
- name: ' - Create a new line item'
  x-api-slug: v3merchantsmidordersorderidline-items-post
  description: Create a new line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-post-openapi.md
- name: ' - Get all line items for an order'
  x-api-slug: v3merchantsmidordersorderidline-items-get
  description: Get all line items for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderidline-items-get-openapi.md
- name: ' - Delete a discount'
  x-api-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
  description: Delete a discount.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscountsdiscountid-delete-openapi.md
- name: ' - Create a discount on an order or line item'
  x-api-slug: v3merchantsmidordersorderiddiscounts-post
  description: Create a discount on an order or line item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-post-openapi.md
- name: ' - Get all discounts for an order'
  x-api-slug: v3merchantsmidordersorderiddiscounts-get
  description: Get all discounts for an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderiddiscounts-get-openapi.md
- name: ' - Delete an order'
  x-api-slug: v3merchantsmidordersorderid-delete
  description: Delete an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-delete-openapi.md
- name: ' - Update an order'
  x-api-slug: v3merchantsmidordersorderid-post
  description: Update an order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-post-openapi.md
- name: ' - Get a single order'
  x-api-slug: v3merchantsmidordersorderid-get
  description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
    for more details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidordersorderid-get-openapi.md
- name: ' - Delete an order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-delete
  description: Delete an order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-delete-openapi.md
- name: ' - Update a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-post
  description: Update a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-post-openapi.md
- name: ' - Get a single order type'
  x-api-slug: v3merchantsmidorder-typesordertypeid-get
  description: Get a single order type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/clover/v3merchantsmidorder-typesordertypeid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://cloudflare.api.gallery.streamdata.io
- type: x-api-stack
  url: http://clover.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/clover
- type: x-developer
  url: https://www.clover.com/developers
- type: x-documentation
  url: https://docs.clover.com/
- type: x-github
  url: https://github.com/clover
- type: x-twitter
  url: https://twitter.com/CloverPOS
- type: x-website
  url: https://www.clover.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---