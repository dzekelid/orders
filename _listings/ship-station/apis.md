---
name: Ship Station
x-slug: ship-station
description: ShipStation is a web-based shipping solution that streamlines the order
  fulfillment process for your online business. ShipStation consolidates orders from
  over 70 ecommerce channels, creates shipping labels, packing slips, and pick lists
  in batch, communicates tracking information to your customers, provides endless
  automation, filters, and views, wireless printing, a mobile app, and a lot more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Orders
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/apis.md
specificationVersion: "0.14"
apis:
- name: Ship Station Developer Portal - List Orders w/o parameters
  x-api-slug: orders-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orders-get-openapi.md
- name: Ship Station Developer Portal - Create/Update Multiple Orders
  x-api-slug: orderscreateorders-post
  description: |-
    This endpoint can be used to create or update multiple orders in one request. If the ``orderKey`` is specified in an order, the existing order with that key will be updated. Note: Only orders in an open status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``) can be updated through this method. ``cancelled`` and ``shipped`` are locked from modification through the API.

    Data Type          |Description
    -------------------|-------------------
    Order, required | An array of [**Order**](http://www.shipstation.com/developer-api/#/reference/model-order) objects (maximum of 100 per request)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderscreateorders-post-openapi.md
- name: Ship Station Developer Portal - List Orders by Tag
  x-api-slug: orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get
  description: |-
    Lists all orders that match the specified status and tag ID.

    Url format with filters:

    ```
    /listbytag?orderStatus={orderStatus}
    &tagId={tagId}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Orders with parameters
  x-api-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get-openapi.md
- name: Ship Station Developer Portal - Add Tag to Order
  x-api-slug: ordersaddtag-post
  description: |-
    Adds a tag to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be tagged.
    ``tagId`` | number, required | Identifies the tag that will be applied to the order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersaddtag-post-openapi.md
- name: Ship Station Developer Portal - Assign User to Order
  x-api-slug: ordersassignuser-post
  description: |-
    Assigns a user to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will be assigned the user.  Please note that if ANY of the orders within the array are not found, no orders will have a user assigned to them.
    ``userId`` | number, required | Identifies the user that will be applied to the orders.  It should contain a GUID of the user to be assigned to the array of orders.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersassignuser-post-openapi.md
- name: Ship Station Developer Portal - Create/Update Order
  x-api-slug: orderscreateorder-post
  description: "If the ``orderKey`` is specified, the method becomes idempotent and
    the existing order with that key will be updated. Note: Only orders in an open
    status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``)
    can be updated through this method. ``cancelled`` and ``shipped`` are locked from
    modification through the API.  The body of this request should specify an [**Order**](https://www.shipstation.com/developer-api/#/reference/model-order)
    object:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n``orderNumber``
    | string, required | A user-defined order number used to identify an order.\n``orderKey``
    | string, optional | A user-provided key that should be unique to each order.
    \ If an orderKey is not provided, ShipStation will create a new order and generate
    a unique orderKey for that order.  If the orderKey *is* provided, the **createorder**
    method will either: create a new order if the provided orderKey is not found,
    or, update the existing order if the orderKey is found.\n``orderDate`` | string,
    required | The date the order was placed.\n``paymentDate`` | string, optional
    | The date the order was paid for.\n``shipByDate`` | string, optional | The date
    the order is to be shipped before or on. This field is a suggested value generated
    by the order source/platform/cart and passed to ShipStation.\n``orderStatus``
    | string, required | The order's status. Possible values: ``awaiting_payment``,
    ``awaiting_shipment``, ``shipped``, ``on_hold``, ``cancelled``\n``customerUsername``
    | string, optional | The customer's username.\n``customerEmail`` | string, optional
    | The customer's email address.\n``billTo`` | Address, required | The recipients
    billing address. Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``shipTo`` | Address, required | The recipient's shipping address. Use
    the [**Address**](http://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``items`` | OrderItem, optional | An array of item objects.  Use an array
    of [**OrderItem**](http://www.shipstation.com/developer-api/#/reference/model-orderitem)
    models.\n``amountPaid`` | number, optional | The total amount paid for the Order.\n``taxAmount``
    | number, optional | The total tax amount for the Order.\n``shippingAmount`` |
    number, optional | Shipping amount paid by the customer, if any.\n``customerNotes``
    | string, optional | Notes left by the customer when placing the order.\n``internalNotes``
    | string, optional | Private notes that are only visible to the seller.\n``gift``
    | boolean, optional | Specifies whether or not this Order is a gift\n``giftMessage``
    | string, optional | Gift message left by the customer when placing the order.\n``paymentMethod``
    | string, optional | Identifies the shipping service selected by the customer
    when placing this order.\n``requestedShippingService`` | string, optional |Identifies
    the shipping service selected by the customer when placing this order. This value
    is given to ShipStation by the marketplace/cart and helps identify what shipping
    service the customer selected upon checkout.\n``carrierCode`` | string, optional
    | The code for the carrier that is to be used(or was used) when this order is
    shipped(was shipped).\n``serviceCode`` | string, optional | The code for the shipping
    service that is to be used(or was used) when this order is shipped(was shipped).\n``packageCode``
    | string, optional | The code for the package type that is to be used(or was used)
    when this order is shipped(was shipped).\n``confirmation`` | string, optional
    | The type of delivery confirmation that is to be used(or was used) when this
    order is shipped(was shipped). Possible values: ``none``, ``delivery``, ``signature``,
    ``adult_signature``, and ``direct_signature``.  ``direct_signature`` is available
    for FedEx only.  \n``shipDate`` | string, optional | The date the order was shipped.\n``weight``
    | Weight, optional | Weight of the order.  Use the [**Weight**](http://www.shipstation.com/developer-api/#/reference/model-weight)
    model.\n``dimensions`` | Dimensions, optional | Dimensions of the order.  Use
    the [**Dimensions**](http://www.shipstation.com/developer-api/#/reference/model-dimensions)
    model.\n``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
    information associated with this order.  Use the [**InsuranceOptions**](http://www.shipstation.com/developer-api/#/reference/model-insuranceoptions)
    model.\n``internationalOptions`` | InternationalOptions, optional | Customs information
    that can be used to generate customs documents for international orders.  Use
    the [**InternationalOptions**](http://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
    model.\n``advancedOptions`` | AdvancedOptions, optional | Various advanced options
    that may be available depending on the shipping carrier that is used to ship the
    order. Use the [**AdvancedOptions**](http://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
    model."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderscreateorder-post-openapi.md
- name: Ship Station Developer Portal - Hold Order Until
  x-api-slug: ordersholduntil-post
  description: |-
    This method will change the status of the given order to On Hold until the date specified, when the status will automatically change to Awaiting Shipment.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be held.
    ``holdUntilDate`` | string, required | Date when order is moved from ``on_hold`` status to ``awaiting_shipment``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersholduntil-post-openapi.md
- name: Ship Station Developer Portal - Mark an Order as Shipped
  x-api-slug: ordersmarkasshipped-post
  description: |-
    Marks an order as shipped without creating a label in ShipStation. The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``orderId`` | number, required | Identifies the order that will be marked as shipped.
     ``carrierCode`` | string, required | Code of the carrier that is marked as having shipped the order.
     ``shipDate`` | string, optional | Date order was shipped.
     ``trackingNumber`` | string, optional | Tracking number of shipment.
     ``notifyCustomer``  | boolean, optional | Specifies whether the customer should be notified of the shipment. Default value: false
     ``notifySalesChannel`` | boolean, optional | Specifies whether the sales channel should be notified of the shipment. Default value: false
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersmarkasshipped-post-openapi.md
- name: Ship Station Developer Portal - Remove Tag from Order
  x-api-slug: ordersremovetag-post
  description: |-
    Removes a tag from the specified order.  The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order whose tag will be removed.
    ``tagId`` | number, required | Identifies the tag to remove.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersremovetag-post-openapi.md
- name: Ship Station Developer Portal - Restore Order from On Hold
  x-api-slug: ordersrestorefromhold-post
  description: |-
    This method will change the status of the given order from On Hold to Awaiting Shipment. This endpoint is used when a holdUntil Date is attached to an order.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be restored to ``awaiting_shipment`` from ``on_hold``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersrestorefromhold-post-openapi.md
- name: Ship Station Developer Portal - Unassign User from Order
  x-api-slug: ordersunassignuser-post
  description: |-
    Unassigns a user from an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will have the user unassigned.  Please note that if ANY of the orders within the array are not found, then no orders will have their users unassigned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersunassignuser-post-openapi.md
- name: Ship Station Developer Portal - Delete Order
  x-api-slug: ordersorderid-delete
  description: Removes order from ShipStation's UI. Note this is a "soft" delete action
    so the order will still exist in the database, but will be set to ``inactive``
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-delete-openapi.md
- name: Ship Station Developer Portal - Get Order
  x-api-slug: ordersorderid-get
  description: Retrieves a single order from the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-get-openapi.md
- name: Ship Station Developer Portal - Add Tag to Order
  x-api-slug: ordersaddtag-post
  description: |-
    Adds a tag to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be tagged.
    ``tagId`` | number, required | Identifies the tag that will be applied to the order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersaddtag-post-openapi.md
- name: Ship Station Developer Portal - Assign User to Order
  x-api-slug: ordersassignuser-post
  description: |-
    Assigns a user to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will be assigned the user.  Please note that if ANY of the orders within the array are not found, no orders will have a user assigned to them.
    ``userId`` | number, required | Identifies the user that will be applied to the orders.  It should contain a GUID of the user to be assigned to the array of orders.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersassignuser-post-openapi.md
- name: Ship Station Developer Portal - Create/Update Order
  x-api-slug: orderscreateorder-post
  description: "If the ``orderKey`` is specified, the method becomes idempotent and
    the existing order with that key will be updated. Note: Only orders in an open
    status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``)
    can be updated through this method. ``cancelled`` and ``shipped`` are locked from
    modification through the API.  The body of this request should specify an [**Order**](https://www.shipstation.com/developer-api/#/reference/model-order)
    object:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n``orderNumber``
    | string, required | A user-defined order number used to identify an order.\n``orderKey``
    | string, optional | A user-provided key that should be unique to each order.
    \ If an orderKey is not provided, ShipStation will create a new order and generate
    a unique orderKey for that order.  If the orderKey *is* provided, the **createorder**
    method will either: create a new order if the provided orderKey is not found,
    or, update the existing order if the orderKey is found.\n``orderDate`` | string,
    required | The date the order was placed.\n``paymentDate`` | string, optional
    | The date the order was paid for.\n``shipByDate`` | string, optional | The date
    the order is to be shipped before or on. This field is a suggested value generated
    by the order source/platform/cart and passed to ShipStation.\n``orderStatus``
    | string, required | The order's status. Possible values: ``awaiting_payment``,
    ``awaiting_shipment``, ``shipped``, ``on_hold``, ``cancelled``\n``customerUsername``
    | string, optional | The customer's username.\n``customerEmail`` | string, optional
    | The customer's email address.\n``billTo`` | Address, required | The recipients
    billing address. Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``shipTo`` | Address, required | The recipient's shipping address. Use
    the [**Address**](http://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``items`` | OrderItem, optional | An array of item objects.  Use an array
    of [**OrderItem**](http://www.shipstation.com/developer-api/#/reference/model-orderitem)
    models.\n``amountPaid`` | number, optional | The total amount paid for the Order.\n``taxAmount``
    | number, optional | The total tax amount for the Order.\n``shippingAmount`` |
    number, optional | Shipping amount paid by the customer, if any.\n``customerNotes``
    | string, optional | Notes left by the customer when placing the order.\n``internalNotes``
    | string, optional | Private notes that are only visible to the seller.\n``gift``
    | boolean, optional | Specifies whether or not this Order is a gift\n``giftMessage``
    | string, optional | Gift message left by the customer when placing the order.\n``paymentMethod``
    | string, optional | Identifies the shipping service selected by the customer
    when placing this order.\n``requestedShippingService`` | string, optional |Identifies
    the shipping service selected by the customer when placing this order. This value
    is given to ShipStation by the marketplace/cart and helps identify what shipping
    service the customer selected upon checkout.\n``carrierCode`` | string, optional
    | The code for the carrier that is to be used(or was used) when this order is
    shipped(was shipped).\n``serviceCode`` | string, optional | The code for the shipping
    service that is to be used(or was used) when this order is shipped(was shipped).\n``packageCode``
    | string, optional | The code for the package type that is to be used(or was used)
    when this order is shipped(was shipped).\n``confirmation`` | string, optional
    | The type of delivery confirmation that is to be used(or was used) when this
    order is shipped(was shipped). Possible values: ``none``, ``delivery``, ``signature``,
    ``adult_signature``, and ``direct_signature``.  ``direct_signature`` is available
    for FedEx only.  \n``shipDate`` | string, optional | The date the order was shipped.\n``weight``
    | Weight, optional | Weight of the order.  Use the [**Weight**](http://www.shipstation.com/developer-api/#/reference/model-weight)
    model.\n``dimensions`` | Dimensions, optional | Dimensions of the order.  Use
    the [**Dimensions**](http://www.shipstation.com/developer-api/#/reference/model-dimensions)
    model.\n``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
    information associated with this order.  Use the [**InsuranceOptions**](http://www.shipstation.com/developer-api/#/reference/model-insuranceoptions)
    model.\n``internationalOptions`` | InternationalOptions, optional | Customs information
    that can be used to generate customs documents for international orders.  Use
    the [**InternationalOptions**](http://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
    model.\n``advancedOptions`` | AdvancedOptions, optional | Various advanced options
    that may be available depending on the shipping carrier that is used to ship the
    order. Use the [**AdvancedOptions**](http://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
    model."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderscreateorder-post-openapi.md
- name: Ship Station Developer Portal - Hold Order Until
  x-api-slug: ordersholduntil-post
  description: |-
    This method will change the status of the given order to On Hold until the date specified, when the status will automatically change to Awaiting Shipment.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be held.
    ``holdUntilDate`` | string, required | Date when order is moved from ``on_hold`` status to ``awaiting_shipment``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersholduntil-post-openapi.md
- name: Ship Station Developer Portal - Mark an Order as Shipped
  x-api-slug: ordersmarkasshipped-post
  description: |-
    Marks an order as shipped without creating a label in ShipStation. The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``orderId`` | number, required | Identifies the order that will be marked as shipped.
     ``carrierCode`` | string, required | Code of the carrier that is marked as having shipped the order.
     ``shipDate`` | string, optional | Date order was shipped.
     ``trackingNumber`` | string, optional | Tracking number of shipment.
     ``notifyCustomer``  | boolean, optional | Specifies whether the customer should be notified of the shipment. Default value: false
     ``notifySalesChannel`` | boolean, optional | Specifies whether the sales channel should be notified of the shipment. Default value: false
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersmarkasshipped-post-openapi.md
- name: Ship Station Developer Portal - Remove Tag from Order
  x-api-slug: ordersremovetag-post
  description: |-
    Removes a tag from the specified order.  The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order whose tag will be removed.
    ``tagId`` | number, required | Identifies the tag to remove.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersremovetag-post-openapi.md
- name: Ship Station Developer Portal - Restore Order from On Hold
  x-api-slug: ordersrestorefromhold-post
  description: |-
    This method will change the status of the given order from On Hold to Awaiting Shipment. This endpoint is used when a holdUntil Date is attached to an order.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be restored to ``awaiting_shipment`` from ``on_hold``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersrestorefromhold-post-openapi.md
- name: Ship Station Developer Portal - Unassign User from Order
  x-api-slug: ordersunassignuser-post
  description: |-
    Unassigns a user from an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will have the user unassigned.  Please note that if ANY of the orders within the array are not found, then no orders will have their users unassigned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersunassignuser-post-openapi.md
- name: Ship Station Developer Portal - Delete Order
  x-api-slug: ordersorderid-delete
  description: Removes order from ShipStation's UI. Note this is a "soft" delete action
    so the order will still exist in the database, but will be set to ``inactive``
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-delete-openapi.md
- name: Ship Station Developer Portal - Get Order
  x-api-slug: ordersorderid-get
  description: Retrieves a single order from the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-get-openapi.md
- name: Ship Station Developer Portal - Get Order
  x-api-slug: ordersorderid-get
  description: Retrieves a single order from the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-get-openapi.md
- name: Ship Station Developer Portal - Delete Order
  x-api-slug: ordersorderid-delete
  description: Removes order from ShipStation's UI. Note this is a "soft" delete action
    so the order will still exist in the database, but will be set to ``inactive``
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersorderid-delete-openapi.md
- name: Ship Station Developer Portal - Unassign User from Order
  x-api-slug: ordersunassignuser-post
  description: |-
    Unassigns a user from an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will have the user unassigned.  Please note that if ANY of the orders within the array are not found, then no orders will have their users unassigned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersunassignuser-post-openapi.md
- name: Ship Station Developer Portal - Restore Order from On Hold
  x-api-slug: ordersrestorefromhold-post
  description: |-
    This method will change the status of the given order from On Hold to Awaiting Shipment. This endpoint is used when a holdUntil Date is attached to an order.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be restored to ``awaiting_shipment`` from ``on_hold``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersrestorefromhold-post-openapi.md
- name: Ship Station Developer Portal - Remove Tag from Order
  x-api-slug: ordersremovetag-post
  description: |-
    Removes a tag from the specified order.  The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order whose tag will be removed.
    ``tagId`` | number, required | Identifies the tag to remove.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersremovetag-post-openapi.md
- name: Ship Station Developer Portal - Mark an Order as Shipped
  x-api-slug: ordersmarkasshipped-post
  description: |-
    Marks an order as shipped without creating a label in ShipStation. The body of this request has the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
     ``orderId`` | number, required | Identifies the order that will be marked as shipped.
     ``carrierCode`` | string, required | Code of the carrier that is marked as having shipped the order.
     ``shipDate`` | string, optional | Date order was shipped.
     ``trackingNumber`` | string, optional | Tracking number of shipment.
     ``notifyCustomer``  | boolean, optional | Specifies whether the customer should be notified of the shipment. Default value: false
     ``notifySalesChannel`` | boolean, optional | Specifies whether the sales channel should be notified of the shipment. Default value: false
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersmarkasshipped-post-openapi.md
- name: Ship Station Developer Portal - Hold Order Until
  x-api-slug: ordersholduntil-post
  description: |-
    This method will change the status of the given order to On Hold until the date specified, when the status will automatically change to Awaiting Shipment.

    The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be held.
    ``holdUntilDate`` | string, required | Date when order is moved from ``on_hold`` status to ``awaiting_shipment``.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersholduntil-post-openapi.md
- name: Ship Station Developer Portal - Create/Update Order
  x-api-slug: orderscreateorder-post
  description: "If the ``orderKey`` is specified, the method becomes idempotent and
    the existing order with that key will be updated. Note: Only orders in an open
    status in ShipStation (``awaiting_payment``,``awaiting_shipment``, and ``on_hold``)
    can be updated through this method. ``cancelled`` and ``shipped`` are locked from
    modification through the API.  The body of this request should specify an [**Order**](https://www.shipstation.com/developer-api/#/reference/model-order)
    object:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n``orderNumber``
    | string, required | A user-defined order number used to identify an order.\n``orderKey``
    | string, optional | A user-provided key that should be unique to each order.
    \ If an orderKey is not provided, ShipStation will create a new order and generate
    a unique orderKey for that order.  If the orderKey *is* provided, the **createorder**
    method will either: create a new order if the provided orderKey is not found,
    or, update the existing order if the orderKey is found.\n``orderDate`` | string,
    required | The date the order was placed.\n``paymentDate`` | string, optional
    | The date the order was paid for.\n``shipByDate`` | string, optional | The date
    the order is to be shipped before or on. This field is a suggested value generated
    by the order source/platform/cart and passed to ShipStation.\n``orderStatus``
    | string, required | The order's status. Possible values: ``awaiting_payment``,
    ``awaiting_shipment``, ``shipped``, ``on_hold``, ``cancelled``\n``customerUsername``
    | string, optional | The customer's username.\n``customerEmail`` | string, optional
    | The customer's email address.\n``billTo`` | Address, required | The recipients
    billing address. Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``shipTo`` | Address, required | The recipient's shipping address. Use
    the [**Address**](http://www.shipstation.com/developer-api/#/reference/model-address)
    model.\n``items`` | OrderItem, optional | An array of item objects.  Use an array
    of [**OrderItem**](http://www.shipstation.com/developer-api/#/reference/model-orderitem)
    models.\n``amountPaid`` | number, optional | The total amount paid for the Order.\n``taxAmount``
    | number, optional | The total tax amount for the Order.\n``shippingAmount`` |
    number, optional | Shipping amount paid by the customer, if any.\n``customerNotes``
    | string, optional | Notes left by the customer when placing the order.\n``internalNotes``
    | string, optional | Private notes that are only visible to the seller.\n``gift``
    | boolean, optional | Specifies whether or not this Order is a gift\n``giftMessage``
    | string, optional | Gift message left by the customer when placing the order.\n``paymentMethod``
    | string, optional | Identifies the shipping service selected by the customer
    when placing this order.\n``requestedShippingService`` | string, optional |Identifies
    the shipping service selected by the customer when placing this order. This value
    is given to ShipStation by the marketplace/cart and helps identify what shipping
    service the customer selected upon checkout.\n``carrierCode`` | string, optional
    | The code for the carrier that is to be used(or was used) when this order is
    shipped(was shipped).\n``serviceCode`` | string, optional | The code for the shipping
    service that is to be used(or was used) when this order is shipped(was shipped).\n``packageCode``
    | string, optional | The code for the package type that is to be used(or was used)
    when this order is shipped(was shipped).\n``confirmation`` | string, optional
    | The type of delivery confirmation that is to be used(or was used) when this
    order is shipped(was shipped). Possible values: ``none``, ``delivery``, ``signature``,
    ``adult_signature``, and ``direct_signature``.  ``direct_signature`` is available
    for FedEx only.  \n``shipDate`` | string, optional | The date the order was shipped.\n``weight``
    | Weight, optional | Weight of the order.  Use the [**Weight**](http://www.shipstation.com/developer-api/#/reference/model-weight)
    model.\n``dimensions`` | Dimensions, optional | Dimensions of the order.  Use
    the [**Dimensions**](http://www.shipstation.com/developer-api/#/reference/model-dimensions)
    model.\n``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
    information associated with this order.  Use the [**InsuranceOptions**](http://www.shipstation.com/developer-api/#/reference/model-insuranceoptions)
    model.\n``internationalOptions`` | InternationalOptions, optional | Customs information
    that can be used to generate customs documents for international orders.  Use
    the [**InternationalOptions**](http://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
    model.\n``advancedOptions`` | AdvancedOptions, optional | Various advanced options
    that may be available depending on the shipping carrier that is used to ship the
    order. Use the [**AdvancedOptions**](http://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
    model."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/orderscreateorder-post-openapi.md
- name: Ship Station Developer Portal - Assign User to Order
  x-api-slug: ordersassignuser-post
  description: |-
    Assigns a user to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderIds`` | number, required | Identifies set of orders that will be assigned the user.  Please note that if ANY of the orders within the array are not found, no orders will have a user assigned to them.
    ``userId`` | number, required | Identifies the user that will be applied to the orders.  It should contain a GUID of the user to be assigned to the array of orders.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersassignuser-post-openapi.md
- name: Ship Station Developer Portal - Add Tag to Order
  x-api-slug: ordersaddtag-post
  description: |-
    Adds a tag to an order.  The body of this request should specify the following attributes:

    Name               |Data Type          |Description
    -------------------|-------------------|-------------------
    ``orderId`` | number, required | Identifies the order that will be tagged.
    ``tagId`` | number, required | Identifies the tag that will be applied to the order.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/orders/master/_listings/ship-station/ordersaddtag-post-openapi.md
x-common:
- type: x-website
  url: http://bit.ly/_ShipStation
- type: x-api-gallery
  url: http://server.density.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ship.station.stack.network
- type: x-blog
  url: https://www.shipstation.com/blog/
- type: x-developer
  url: https://shipstation.docs.apiary.io/#
- type: x-github
  url: https://github.com/shipstation
- type: x-partners
  url: https://www.shipstation.com/partners/
- type: x-pricing
  url: https://www.shipstation.com/pricing/
- type: x-twitter
  url: https://twitter.com/ShipStation
- type: x-website
  url: http://shipstation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---