---
swagger: "2.0"
x-collection-name: Ship Station
x-complete: 0
info:
  title: Ship Station Create/Update Order
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
  /orders/addtag:
    post:
      summary: Add Tag to Order
      description: |-
        Adds a tag to an order.  The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderId`` | number, required | Identifies the order that will be tagged.
        ``tagId`` | number, required | Identifies the tag that will be applied to the order.
      operationId: orders.addtag.post
      x-api-path-slug: ordersaddtag-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Tag
      - To
      - Order
  /orders/assignuser:
    post:
      summary: Assign User to Order
      description: |-
        Assigns a user to an order.  The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderIds`` | number, required | Identifies set of orders that will be assigned the user.  Please note that if ANY of the orders within the array are not found, no orders will have a user assigned to them.
        ``userId`` | number, required | Identifies the user that will be applied to the orders.  It should contain a GUID of the user to be assigned to the array of orders.
      operationId: orders.assignuser.post
      x-api-path-slug: ordersassignuser-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Assign
      - User
      - To
      - Order
  /orders/createorder:
    post:
      summary: Create/Update Order
      description: "If the ``orderKey`` is specified, the method becomes idempotent
        and the existing order with that key will be updated. Note: Only orders in
        an open status in ShipStation (``awaiting_payment``,``awaiting_shipment``,
        and ``on_hold``) can be updated through this method. ``cancelled`` and ``shipped``
        are locked from modification through the API.  The body of this request should
        specify an [**Order**](https://www.shipstation.com/developer-api/#/reference/model-order)
        object:\n\nName               |Data Type          |Description\n-------------------|-------------------|-------------------\n``orderNumber``
        | string, required | A user-defined order number used to identify an order.\n``orderKey``
        | string, optional | A user-provided key that should be unique to each order.
        \ If an orderKey is not provided, ShipStation will create a new order and
        generate a unique orderKey for that order.  If the orderKey *is* provided,
        the **createorder** method will either: create a new order if the provided
        orderKey is not found, or, update the existing order if the orderKey is found.\n``orderDate``
        | string, required | The date the order was placed.\n``paymentDate`` | string,
        optional | The date the order was paid for.\n``shipByDate`` | string, optional
        | The date the order is to be shipped before or on. This field is a suggested
        value generated by the order source/platform/cart and passed to ShipStation.\n``orderStatus``
        | string, required | The order's status. Possible values: ``awaiting_payment``,
        ``awaiting_shipment``, ``shipped``, ``on_hold``, ``cancelled``\n``customerUsername``
        | string, optional | The customer's username.\n``customerEmail`` | string,
        optional | The customer's email address.\n``billTo`` | Address, required |
        The recipients billing address. Use the [**Address**](https://www.shipstation.com/developer-api/#/reference/model-address)
        model.\n``shipTo`` | Address, required | The recipient's shipping address.
        Use the [**Address**](http://www.shipstation.com/developer-api/#/reference/model-address)
        model.\n``items`` | OrderItem, optional | An array of item objects.  Use an
        array of [**OrderItem**](http://www.shipstation.com/developer-api/#/reference/model-orderitem)
        models.\n``amountPaid`` | number, optional | The total amount paid for the
        Order.\n``taxAmount`` | number, optional | The total tax amount for the Order.\n``shippingAmount``
        | number, optional | Shipping amount paid by the customer, if any.\n``customerNotes``
        | string, optional | Notes left by the customer when placing the order.\n``internalNotes``
        | string, optional | Private notes that are only visible to the seller.\n``gift``
        | boolean, optional | Specifies whether or not this Order is a gift\n``giftMessage``
        | string, optional | Gift message left by the customer when placing the order.\n``paymentMethod``
        | string, optional | Identifies the shipping service selected by the customer
        when placing this order.\n``requestedShippingService`` | string, optional
        |Identifies the shipping service selected by the customer when placing this
        order. This value is given to ShipStation by the marketplace/cart and helps
        identify what shipping service the customer selected upon checkout.\n``carrierCode``
        | string, optional | The code for the carrier that is to be used(or was used)
        when this order is shipped(was shipped).\n``serviceCode`` | string, optional
        | The code for the shipping service that is to be used(or was used) when this
        order is shipped(was shipped).\n``packageCode`` | string, optional | The code
        for the package type that is to be used(or was used) when this order is shipped(was
        shipped).\n``confirmation`` | string, optional | The type of delivery confirmation
        that is to be used(or was used) when this order is shipped(was shipped). Possible
        values: ``none``, ``delivery``, ``signature``, ``adult_signature``, and ``direct_signature``.
        \ ``direct_signature`` is available for FedEx only.  \n``shipDate`` | string,
        optional | The date the order was shipped.\n``weight`` | Weight, optional
        | Weight of the order.  Use the [**Weight**](http://www.shipstation.com/developer-api/#/reference/model-weight)
        model.\n``dimensions`` | Dimensions, optional | Dimensions of the order.  Use
        the [**Dimensions**](http://www.shipstation.com/developer-api/#/reference/model-dimensions)
        model.\n``insuranceOptions`` | InsuranceOptions, optional | The shipping insurance
        information associated with this order.  Use the [**InsuranceOptions**](http://www.shipstation.com/developer-api/#/reference/model-insuranceoptions)
        model.\n``internationalOptions`` | InternationalOptions, optional | Customs
        information that can be used to generate customs documents for international
        orders.  Use the [**InternationalOptions**](http://www.shipstation.com/developer-api/#/reference/model-internationaloptions)
        model.\n``advancedOptions`` | AdvancedOptions, optional | Various advanced
        options that may be available depending on the shipping carrier that is used
        to ship the order. Use the [**AdvancedOptions**](http://www.shipstation.com/developer-api/#/reference/model-advancedoptions)
        model."
      operationId: orders.createorder.post
      x-api-path-slug: orderscreateorder-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Order
  /orders/holduntil:
    post:
      summary: Hold Order Until
      description: |-
        This method will change the status of the given order to On Hold until the date specified, when the status will automatically change to Awaiting Shipment.

        The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderId`` | number, required | Identifies the order that will be held.
        ``holdUntilDate`` | string, required | Date when order is moved from ``on_hold`` status to ``awaiting_shipment``.
      operationId: orders.holduntil.post
      x-api-path-slug: ordersholduntil-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hold
      - Order
      - Until
  /orders/markasshipped:
    post:
      summary: Mark an Order as Shipped
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
      operationId: orders.markasshipped.post
      x-api-path-slug: ordersmarkasshipped-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Order
      - As
      - Shipped
  /orders/removetag:
    post:
      summary: Remove Tag from Order
      description: |-
        Removes a tag from the specified order.  The body of this request has the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderId`` | number, required | Identifies the order whose tag will be removed.
        ``tagId`` | number, required | Identifies the tag to remove.
      operationId: orders.removetag.post
      x-api-path-slug: ordersremovetag-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Tag
      - From
      - Order
  /orders/restorefromhold:
    post:
      summary: Restore Order from On Hold
      description: |-
        This method will change the status of the given order from On Hold to Awaiting Shipment. This endpoint is used when a holdUntil Date is attached to an order.

        The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderId`` | number, required | Identifies the order that will be restored to ``awaiting_shipment`` from ``on_hold``.
      operationId: orders.restorefromhold.post
      x-api-path-slug: ordersrestorefromhold-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Restore
      - Order
      - From
      - "On"
      - Hold
  /orders/unassignuser:
    post:
      summary: Unassign User from Order
      description: |-
        Unassigns a user from an order.  The body of this request should specify the following attributes:

        Name               |Data Type          |Description
        -------------------|-------------------|-------------------
        ``orderIds`` | number, required | Identifies set of orders that will have the user unassigned.  Please note that if ANY of the orders within the array are not found, then no orders will have their users unassigned.
      operationId: orders.unassignuser.post
      x-api-path-slug: ordersunassignuser-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - User
      - From
      - Order
  /orders/{orderId}:
    delete:
      summary: Delete Order
      description: Removes order from ShipStation's UI. Note this is a "soft" delete
        action so the order will still exist in the database, but will be set to ``inactive``
      operationId: orders.orderId.delete
      x-api-path-slug: ordersorderid-delete
      parameters:
      - in: path
        name: orderId
        description: The system generated identifier for the order
      responses:
        200:
          description: OK
      tags:
      - Order
    get:
      summary: Get Order
      description: Retrieves a single order from the database.
      operationId: orders.orderId.get
      x-api-path-slug: ordersorderid-get
      parameters:
      - in: path
        name: orderId
        description: The system generated identifier for the order
      responses:
        200:
          description: OK
      tags:
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