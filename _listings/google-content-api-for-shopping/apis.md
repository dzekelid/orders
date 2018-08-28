---
name: Google Content API for Shopping
x-slug: google-content-api-for-shopping
description: 'API allowing retailers to manage their product feed content programmatically.
  Providing item-level data quality information: See if an item was disapproved because
  a landing page URL isn&rsquo;t working on a mobile device or if unique product identifiers
  are inaccurate. Faster pricing and availability updates: Ensure customers have the
  latest price-points and know what&rsquo;s in-stock before they click through to
  your site. More integration options: The newer API supports a broader choice of
  programming languages and data formats.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/apis.md
specificationVersion: "0.14"
apis:
- name: Content API for Shopping - Orders
  x-api-slug: ordersbatch-post
  description: Retrieves or modifies multiple orders in a single request. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/ordersbatch-post-openapi.md
- name: Content API for Shopping - Get Orders
  x-api-slug: merchantidorders-get
  description: Lists the orders in your Merchant Center account. This method can only
    be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidorders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidorders-get-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersorderid-get
  description: Retrieves an order from your Merchant Center account. This method can
    only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderid-get-openapi.md
- name: Content API for Shopping - Acknowledge Order
  x-api-slug: merchantidordersorderidacknowledge-post
  description: Marks an order as acknowledged. This method can only be called for
    non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidacknowledge-post-openapi.md
- name: Content API for Shopping - Cancel Order
  x-api-slug: merchantidordersorderidcancel-post
  description: Cancels all line items in an order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancel-post-openapi.md
- name: Content API for Shopping - Cancel Order Line Item
  x-api-slug: merchantidordersorderidcancellineitem-post
  description: Cancels a line item. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancellineitem-post-openapi.md
- name: Content API for Shopping - Refund Order
  x-api-slug: merchantidordersorderidrefund-post
  description: Refund a portion of the order, up to the full amount paid. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidrefund-post-openapi.md
- name: Content API for Shopping - Update Merchant Order ID
  x-api-slug: merchantidordersorderidupdatemerchantorderid-post
  description: Updates the merchant order ID for a given order. This method can only
    be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdatemerchantorderid-post-openapi.md
- name: Content API for Shopping - Update order Shippment
  x-api-slug: merchantidordersorderidupdateshipment-post
  description: Updates a shipment's status, carrier, and/or tracking ID. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdateshipment-post-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersbymerchantidmerchantorderid-get
  description: Retrieves an order using merchant order id. This method can only be
    called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersbymerchantidmerchantorderid-get-openapi.md
- name: Content API for Shopping - Create Test Order
  x-api-slug: merchantidtestorders-post
  description: Sandbox only. Creates a test order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestorders-post-openapi.md
- name: Content API for Shopping - Update Test Order
  x-api-slug: merchantidtestordersorderidadvance-post
  description: Sandbox only. Moves a test order from state "inProgress" to state "pendingShipment".
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordersorderidadvance-post-openapi.md
- name: Content API for Shopping - Get Test Order
  x-api-slug: merchantidtestordertemplatestemplatename-get
  description: Sandbox only. Retrieves an order template that can be used to quickly
    create a new order in sandbox. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordertemplatestemplatename-get-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersorderid-get
  description: Retrieves an order from your Merchant Center account. This method can
    only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderid-get-openapi.md
- name: Content API for Shopping - Acknowledge Order
  x-api-slug: merchantidordersorderidacknowledge-post
  description: Marks an order as acknowledged. This method can only be called for
    non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidacknowledge-post-openapi.md
- name: Content API for Shopping - Cancel Order
  x-api-slug: merchantidordersorderidcancel-post
  description: Cancels all line items in an order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancel-post-openapi.md
- name: Content API for Shopping - Cancel Order Line Item
  x-api-slug: merchantidordersorderidcancellineitem-post
  description: Cancels a line item. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancellineitem-post-openapi.md
- name: Content API for Shopping - Refund Order
  x-api-slug: merchantidordersorderidrefund-post
  description: Refund a portion of the order, up to the full amount paid. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidrefund-post-openapi.md
- name: Content API for Shopping - Update Merchant Order ID
  x-api-slug: merchantidordersorderidupdatemerchantorderid-post
  description: Updates the merchant order ID for a given order. This method can only
    be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdatemerchantorderid-post-openapi.md
- name: Content API for Shopping - Update order Shippment
  x-api-slug: merchantidordersorderidupdateshipment-post
  description: Updates a shipment's status, carrier, and/or tracking ID. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdateshipment-post-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersbymerchantidmerchantorderid-get
  description: Retrieves an order using merchant order id. This method can only be
    called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersbymerchantidmerchantorderid-get-openapi.md
- name: Content API for Shopping - Create Test Order
  x-api-slug: merchantidtestorders-post
  description: Sandbox only. Creates a test order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestorders-post-openapi.md
- name: Content API for Shopping - Update Test Order
  x-api-slug: merchantidtestordersorderidadvance-post
  description: Sandbox only. Moves a test order from state "inProgress" to state "pendingShipment".
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordersorderidadvance-post-openapi.md
- name: Content API for Shopping - Get Test Order
  x-api-slug: merchantidtestordertemplatestemplatename-get
  description: Sandbox only. Retrieves an order template that can be used to quickly
    create a new order in sandbox. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordertemplatestemplatename-get-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersorderid-get
  description: Retrieves an order from your Merchant Center account. This method can
    only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderid-get-openapi.md
- name: Content API for Shopping - Acknowledge Order
  x-api-slug: merchantidordersorderidacknowledge-post
  description: Marks an order as acknowledged. This method can only be called for
    non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidacknowledge-post-openapi.md
- name: Content API for Shopping - Cancel Order
  x-api-slug: merchantidordersorderidcancel-post
  description: Cancels all line items in an order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancel-post-openapi.md
- name: Content API for Shopping - Cancel Order Line Item
  x-api-slug: merchantidordersorderidcancellineitem-post
  description: Cancels a line item. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidcancellineitem-post-openapi.md
- name: Content API for Shopping - Refund Order
  x-api-slug: merchantidordersorderidrefund-post
  description: Refund a portion of the order, up to the full amount paid. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidrefund-post-openapi.md
- name: Content API for Shopping - Update Merchant Order ID
  x-api-slug: merchantidordersorderidupdatemerchantorderid-post
  description: Updates the merchant order ID for a given order. This method can only
    be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdatemerchantorderid-post-openapi.md
- name: Content API for Shopping - Update order Shippment
  x-api-slug: merchantidordersorderidupdateshipment-post
  description: Updates a shipment's status, carrier, and/or tracking ID. This method
    can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersorderidupdateshipment-post-openapi.md
- name: Content API for Shopping - Get Order
  x-api-slug: merchantidordersbymerchantidmerchantorderid-get
  description: Retrieves an order using merchant order id. This method can only be
    called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidordersbymerchantidmerchantorderid-get-openapi.md
- name: Content API for Shopping - Create Test Order
  x-api-slug: merchantidtestorders-post
  description: Sandbox only. Creates a test order. This method can only be called
    for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestorders-post-openapi.md
- name: Content API for Shopping - Update Test Order
  x-api-slug: merchantidtestordersorderidadvance-post
  description: Sandbox only. Moves a test order from state "inProgress" to state "pendingShipment".
    This method can only be called for non-multi-client accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordersorderidadvance-post-openapi.md
- name: Content API for Shopping - Get Test Order
  x-api-slug: merchantidtestordertemplatestemplatename-get
  description: Sandbox only. Retrieves an order template that can be used to quickly
    create a new order in sandbox. This method can only be called for non-multi-client
    accounts.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-shopping-API1.jpg
  humanURL: https://developers.google.com/shopping-content/v2/quickstart
  baseURL: ://www.googleapis.com//content/v2
  tags: Shopping, Commerce, Content, Google APIs, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/google-content-api-for-shopping/merchantidtestordertemplatestemplatename-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.container.engine.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.content.api.for.shopping.stack.network
- type: x-best-practices
  url: https://developers.google.com/shopping-content/v2/best-practices
- type: x-code
  url: https://developers.google.com/shopping-content/v2/libraries
- type: x-testing
  url: https://developers.google.com/shopping-content/v2/how-tos/testing
- type: x-website
  url: https://developers.google.com/shopping-content/v2/quickstart
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---