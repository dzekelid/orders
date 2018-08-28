---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Delete an order type
  version: 1.0.0
  description: Delete an order type.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/orders:
    get:
      summary: Gets a list of orders
      description: Returns a list of orders. See https://docs.clover.com/build/working-with-orders/
        for more details.
      operationId: GetOrders
      x-api-path-slug: v3merchantsmidorders-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, serviceCharge, discounts, credits,
          payments, refunds]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
    post:
      summary: Create an order
      description: Only supports basic order creation. Valid fields are limited to
        taxRemoved, note, title, and orderType. Adding line items must be done in
        separate calls.
      operationId: CreateOrder
      x-api-path-slug: v3merchantsmidorders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
  /v3/merchants/{mId}/employees/{empId}/orders:
    get:
      summary: Get all orders for an employee
      description: Get all orders for an employee.
      operationId: GetEmployeeOrders
      x-api-path-slug: v3merchantsmidemployeesempidorders-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: query
        name: filter
        description: 'Filter fields: [lineItems, customers, payments, credits, refunds,
          serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Orders
  /v3/merchants/{mId}/orders/{orderId}:
    get:
      summary: Get a single order
      description: Returns a single order. See https://docs.clover.com/build/working-with-orders/
        for more details.
      operationId: GetOrder
      x-api-path-slug: v3merchantsmidordersorderid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
    post:
      summary: Update an order
      description: Update an order.
      operationId: UpdateOrder
      x-api-path-slug: v3merchantsmidordersorderid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [lineItems, customers, payments, credits,
          refunds, serviceCharge, discounts]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
    delete:
      summary: Delete an order
      description: Delete an order.
      operationId: DeleteOrder
      x-api-path-slug: v3merchantsmidordersorderid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
  /v3/merchants/{mId}/orders/{orderId}/discounts:
    get:
      summary: Get all discounts for an order
      description: Get all discounts for an order.
      operationId: GetOrderDiscounts
      x-api-path-slug: v3merchantsmidordersorderiddiscounts-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
    post:
      summary: Create a discount on an order or line item
      description: Create a discount on an order or line item.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmidordersorderiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
  /v3/merchants/{mId}/orders/{orderId}/discounts/{discountId}:
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: RemoveDiscount
      x-api-path-slug: v3merchantsmidordersorderiddiscountsdiscountid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Discounts
      - DiscountId
  /v3/merchants/{mId}/orders/{orderId}/line_items:
    get:
      summary: Get all line items for an order
      description: Get all line items for an order.
      operationId: GetOrderLineItems
      x-api-path-slug: v3merchantsmidordersorderidline-items-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
    post:
      summary: Create a new line item
      description: Create a new line item.
      operationId: CreateLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}:
    get:
      summary: Get a line item
      description: Get a line item.
      operationId: GetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    post:
      summary: Update a line item
      description: Update a line item.
      operationId: UpdateOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [employee, orderType, discounts, modifications,
          taxRates, payments]'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
    delete:
      summary: Void a line item
      description: Void a line item.
      operationId: DeleteOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts:
    post:
      summary: Create a discount on an order or line item
      description: Create a discount on an order or line item.
      operationId: CreateDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscounts-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/discounts/{discountId}:
    delete:
      summary: Delete a discount
      description: Delete a discount.
      operationId: RemoveDiscount
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemiddiscountsdiscountid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: discountId
        description: Discount Id
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Discounts
      - DiscountId
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications:
    post:
      summary: Apply a modification to a line item
      description: 'Create a modification, a record of a modifier as it exists at
        the time it is applied to the lineItem. To view current modifications use
        an ''expand=modifications'' query parameter on the lineItem. To learn more
        about applying a modification see: https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
      operationId: ApplyModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
  /v3/merchants/{mId}/orders/{orderId}/line_items/{lineItemId}/modifications/{modificationId}:
    delete:
      summary: Remove a modification from a line item
      description: Delete a modification by UUID, removing the record of an applied
        modification
      operationId: RemoveModification
      x-api-path-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: modificationId
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - LineItemId
      - Modifications
      - ModificationId
  /v3/merchants/{mId}/orders/{orderId}/bulk_line_items:
    post:
      summary: Create multiple line items in bulk.
      description: Create multiple line items in bulk..
      operationId: BulkCreateLineItems
      x-api-path-slug: v3merchantsmidordersorderidbulk-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Bulk
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/payments:
    post:
      summary: Create a payment record on an order
      description: Create a payment record on an order.
      operationId: CreatePaymentForOrder
      x-api-path-slug: v3merchantsmidordersorderidpayments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Payments
    get:
      summary: Get all payments for an order
      description: Get all payments for an order.
      operationId: GetOrderPayments
      x-api-path-slug: v3merchantsmidordersorderidpayments-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [cardTransaction, dccInfo, germanInfo, appTracking,
          taxRates, lineItemPayments, refunds, order, tender, employee, transactionInfo]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, voidReason, cardTransaction'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Payments
  /v3/merchants/{mId}/modifier_group_sort_orders:
    post:
      summary: Update the priorities for a collection of up to 200 modifier groups
        at a time
      description: Update the priorities for a collection of up to 200 modifier groups
        at a time.
      operationId: UpdateModifierGroupSortOrders
      x-api-path-slug: v3merchantsmidmodifier-group-sort-orders-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Modifier
      - Group
      - Sort
      - Orders
  /v3/merchants/{mId}/orders/{orderId}/service_charge/:
    post:
      summary: ""
      description: .
      operationId: ApplyServiceCharge
      x-api-path-slug: v3merchantsmidordersorderidservice-charge-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Service
      - Charge
  /v3/merchants/{mId}/orders/{orderId}/service_charge/{chargeId}:
    delete:
      summary: Remove service charge from an order
      description: Remove service charge from an order.
      operationId: RemoveServiceCharge
      x-api-path-slug: v3merchantsmidordersorderidservice-chargechargeid-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: chargeId
        description: Service Charge Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Service
      - Charge
      - ChargeId
  /v3/merchants/{mId}/orders/{orderId}/voided_line_items:
    post:
      summary: Void a line item
      description: Void a line item.
      operationId: VoidOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidvoided-line-items-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Voided
      - Line
      - Items
  /v3/merchants/{mId}/orders/{orderId}/line_items/{oldLineItemId}/exchange/{lineItemId}:
    post:
      summary: Create or exchange a line item
      description: Create or exchange a line item.
      operationId: SetOrderLineItem
      x-api-path-slug: v3merchantsmidordersorderidline-itemsoldlineitemidexchangelineitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lineItemId
        description: Line Item Id
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: oldLineItemId
        description: Old Line Item Id
      - in: path
        name: orderId
        description: Order Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Orders
      - OrderId
      - Line
      - Items
      - OldLineItemId
      - Exchange
      - LineItemId
  /v3/merchants/{mId}/order_types:
    get:
      summary: Get all order types for a merchant
      description: Merchants have the ability to create custom order types via the
        Setup App (https://www.clover.com/setupapp). These custom order types can
        be associated with a System Order Type (see /v3/merchants/{mId}/system_order_types).
        Custom Order Types can support items in all categories (filterCategories=false)
        or a subset of the merchant's categories (filterCategories=true and categories
        property contains the list of supported categories). Note that when expanding
        the categories for an order type, they will only be returned if this orderType
        only supports a subset of the categories (filterCategories=true). If the orderType
        supports all categories (filterCategories=false) then you should make a GET
        request to /v3/merchants/{mId}/categories.
      operationId: GetOrderTypes
      x-api-path-slug: v3merchantsmidorder-types-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: query
        name: filter
        description: 'Filter fields: [id, deletedTime]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
    post:
      summary: Create Order Type For Merchant
      description: Create order type for merchant.
      operationId: CreateOrderType
      x-api-path-slug: v3merchantsmidorder-types-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
  /v3/merchants/{mId}/order_types/{orderTypeId}:
    get:
      summary: Get a single order type
      description: Get a single order type.
      operationId: GetOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
    post:
      summary: Update a single order type
      description: Update a single order type.
      operationId: UpdateOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [hours, attributes, categories]'
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
    delete:
      summary: Delete an order type
      description: Delete an order type.
      operationId: DeleteOrderType
      x-api-path-slug: v3merchantsmidorder-typesordertypeid-delete
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      - in: path
        name: orderTypeId
        description: Order Type Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Types
      - OrderTypeId
  /v3/merchants/{mId}/order_type_categories:
    post:
      summary: Create or delete a order type category
      description: Create or delete a order type category.
      operationId: CreateOrDeleteOrderTypeCategories
      x-api-path-slug: v3merchantsmidorder-type-categories-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Type
      - Categories
  /v3/merchants/{mId}/system_order_types:
    get:
      summary: Return a list of system order types
      description: Merchants can create custom Order Types via "/v3/merchants/{mId}/order_types".
        It is useful to associate these custom order types with particular system
        order types in order to group things functionally. For example, a merchant
        may have a "Lunch Take-Out" order type and a "Dinner Take-Out" order type.
        These two order types can be associated with the "TAKE-OUT-TYPE" system order
        type so that applications can understand that they are both take-out order
        types.
      operationId: GetSystemOrderTypes
      x-api-path-slug: v3merchantsmidsystem-order-types-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - System
      - Order
      - Types
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