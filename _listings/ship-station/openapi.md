swagger: "2.0"
x-collection-name: Ship Station
x-complete: 1
info:
  title: Ship Station Developer Portal
  description: -integrating-with-shipstationshipstation-strives-to-streamline-shipping-for-online-sellers-no-matter-where-they-sell-their-products-online--we-are-continuously-adding-new-marketplaces-shopping-carts-and-integration-tools-because-we-know-the-ecommerce-space-is-growing--as-a-result-weve-worked-hard-to-provide-developer-resources-to-build-custom-integrations-with-shipstation---if-youre-interested-in-becoming-a-partner-of-ours-drop-us-a-line-by-filling-out-this-formhttpwww-shipstation-compartnersshipstationapicustomstore-and-well-get-in-touch-there-are-two-methods-to-integrate-with-shipstation-custom-store-integration-shipstation-api-custom-store-integrationlooking-for-a-more-1to1-relationship-between-shipstation-and-your-chosen-selling-platform-the-custom-store-integration-is-the-ticket--our-custom-store-integration-is-just-like-any-of-our-other-selling-channel-integration-and-could-be-eligible-based-on-internal-review-as-a-branded-option-within-the-shipstation-admin--it-also-allows-the-user-to-sync-orders-within-shipstation-in-a-single-click-in-addition-to-shipstation-automatically-sending-shipment-status-and-tracking-information-updates-back-to-your-cart-or-marketplace-once-a-label-is-created--its-the-best-way-to-sync-up-orders-with-shipstation-and-have-the-most-seamless-experience-the-custom-store-allows-you-to-perform-two-major-functions-provide-order-information-to-shipstation-including-recipient-address-products-customers-etc--receive-tracking-information-when-an-order-is-shipped-including-shipping-method-shipping-status-tracking-number-and-moreto-integrate-with-the-custom-store-you-must-expose-a-web-page-that-renders-xml-that-adheres-to-the-specification-defined-in-the-custom-store-integration-guide--we-refer-to-this-page-as-your-xml-endpoint--if-you-can-provide-us-an-xml-endpoint-we-can-pull-data-from-your-endpoint-just-like-we-do-with-other-marketplaces-like-ebay-and-amazon-to-find-out-more-about-our-custom-store-integration-click-here-custom-store-integration-guidehttpshelp-shipstation-comhcenusarticles205928478-shipstation-apiour-api-is-available-for-any-plan-and-allows-for-read-access-to-almost-all-data-in-your-account-and-write-access-to-create-specific-objects-like-orders-customers-and-products--the-api-is-a-great-way-to-get-data-directly-to-and-from-shipstation-like-creating-products-customers-and-querying-order--shipping-data--please-note-that-an-api-integration-will-not-allow-you-to-use-your-own-marketplaceid-that-could-eventually-be-branded-with-your-companys-logo-see-the-custom-store-integration-above-for-that-functionality-this-api-allows-developers-to-build-applications-that-interface-with-the-shipstation-platform--the-api-can-be-used-to-automate-many-tasks-including-managing-orders-managing-shipments-creating-shipping-labels-retrieving-shipping-rates-and-moreto-learn-more-about-our-api-please-review-our-api-documentation-below--which-one-should-i-pickthe-method-thats-right-for-your-integration-very-much-depends-on-the-type-of-integration-youre-planning-on-implementing--a-custom-store-allows-shipstation-to-pull-order-information-from-your-platform-the-very-same-way-we-pull-data-from-marketplaces-such-as-ebay-amazon-and-shopify--once-an-order-has-been-shipped-in-shipstation-shipstation-automatically-pushes-tracking-information-back-to-your-custom-store--though-the-functionality-afforded-by-this-approach-is-limited-to-these-2-main-functions-much-of-the-heavy-lifting-is-performed-by-shipstation--importing-orders-and-sending-tracking-information-is-performed-automatically-by-shipstation-as-long-as-your-xml-endpoint-is-available-to-receive-our-data-an-api-integration-on-the-other-hand-exposes-much-more-functionality-but-requires-that-the-developer-do-much-of-the-heavy-lifting--orders-must-be-pushed-to-shipstation-by-using-our-orderscreateorder-endpoint---the-api-allows-developers-to-perform-functions-such-as-tagging-an-order-shipping-an-order-creating-a-shipping-label-without-an-order-retrieving-shipping-rates-adding-funds-to-a-carrier-account-creating-a-warehouse-listing-products-and-much-more---the-functionality-the-api-affords-are-typical-actions-that-a-user-would-perform-if-using-the-web-app--considerations-will-your-integration-be-the-main-order-management-tool-for-the-online-seller--if-so-the-apis-broader-range-of-functionality-may-be-the-best-option--would-you-like-your-store-integration-to-be-a-branded-marketplace-within-the-shipstation-admin-when-you-integrate-using-the-custom-store-integration-you-could-be-eligible-to-have-your-company-branded-within-the-shipstation-admin--a-branded-store-could-have-the-plugins-logo-in-the-appas-well-as-an-easier-store-setup-order-sync-and-reporting--please-note-shipstation-makes-the-final-decision-based-on-integration-and-partner-requirements-on-which-custom-stores-are-branded-within-our-application--shipstation-api-requirements-end-pointendpoints-are-located-at-the-following-domain-httpsssapi-shipstation-com-and-will-need-to-have-a-specific-reference-added-to-return-data--please-note-you-cannot-access-this-url-directly-and-must-reference-one-of-the-specific-endpoints-below--authenticationthe-shipstation-api-uses-basic-http-authenticationhttpen-wikipedia-orgwikibasic-access-authentication--use-your-shipstation-api-key-as-the-username-and-api-secret-as-the-password---you-can-find-your-api-key-as-the-username-and-api-secret-under-settings-at-httpsss-shipstation-comsettingsapi--the-authorization-header-is-constructed-as-follows-username-api-key-and-password-api-secret-are-combined-into-a-string-usernamepassword-the-resulting-string-is-then-encoded-using-the-rfc2045mime-variant-of-base64-except-not-limited-to-76-charline-the-authorization-method-and-a-space-i-e--basic--is-then-put-before-the-encoded-string-for-example-if-the-api-key-given-is-shipstation-and-the-api-secret-is-rocks-then-the-header-is-formed-as-follows-authorization-basic-u2hpcfn0yxrpb246um9ja3m-api-rate-limitsin-an-effort-to-ensure-consistent-application-performance-and-increased-scalability-we-have-implemented-rate-limiting-on-the-shipstation-api---your-integration-will-need-to-be-able-to-handle-http-rate-limiting-status-messages-as-defined-belowresponse-headersall-responses-will-include-headers-with-status-information-about-rate-limiting-1--xratelimitlimit-the-maximum-number-of-requests-per-minute-to-the-endpoint2--xratelimitremaining-the-available-requests-remaining-in-the-current-window3--xratelimitreset-the-number-of-seconds-remaining-until-the-next-window-beginshitting-the-limitif-your-application-hits-the-rate-limit-an-http-429-will-be-returned-with-this-body----message-too-many-requestsand-these-headers-assuming-it-is-40-seconds-into-the-current-window----xratelimitlimit-60----xratelimitremaining-0----xratelimitreset-20when-the-limit-is-reached-your-application-should-stop-making-requests-until-xratelimitreset-seconds-have-elapsed--the-current-rate-limit-for-each-set-of-the-api-key-and-secret-is-40-requests-per-minute-if-you-have-any-issues-with-the-api-please-email-us-at-apisupportshipstation-com-server-responsesstatus-code--description200--ok--the-request-was-successful-some-api-calls-may-return-201-instead-201--created--the-request-was-successful-and-a-resource-was-created-204--no-content--the-request-was-successful-but-there-is-no-representation-to-return-that-is-the-response-is-empty-400--bad-request---the-request-could-not-be-understood-or-was-missing-required-parameters-401--unauthorized---authentication-failed-or-user-does-not-have-permissions-for-the-requested-operation-403--forbidden--access-denied-404--not-found---resource-was-not-found-405--method-not-allowed---requested-method-is-not-supported-for-the-specified-resource-429--too-many-requests--exceeded-shipstation-api-limits--when-the-limit-is-reached-your-application-should-stop-making-requests-until-xratelimitreset-seconds-have-elapsed-500--internal-server-error--shipstation-has-encountered-an-error--datetime-format-and-time-zoneshipstation-uses-the-iso-8601-combined-format-for-datetime-stamps-being-submitted-to-and-returned-from-the-api--please-be-sure-to-submit-all-datetime-values-as-followsyyyymmdd-hhmmss-24-hour-notation--example--20161129-235959the-time-zone-represented-in-all-api-responses-is-pstpdt--similarly-shipstation-asks-that-you-make-all-time-zone-convertions-and-submit-any-datetime-requests-in-pstpdt-
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