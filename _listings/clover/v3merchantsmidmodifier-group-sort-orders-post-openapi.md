---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Update the priorities for a collection of up to 200 modifier groups
    at a time
  version: 1.0.0
  description: Update the priorities for a collection of up to 200 modifier groups
    at a time.
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