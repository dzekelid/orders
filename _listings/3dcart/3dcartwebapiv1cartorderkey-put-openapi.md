---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart This method is used to update a single cart record in the database.
    The {orderkey} parameter specifies which cart record to update.
  version: 1.0.0
  description: This method is used to update a single cart record in the database.
    the {orderkey} parameter specifies which cart record to update..
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Orders:
    put:
      summary: This method is used to update multiple orders in the database. No URL
        parameters should be included.
      description: This method is used to update multiple orders in the database.
        no url parameters should be included..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1orders-put
      parameters:
      - in: body
        name: orders
        description: A Json or XML object containing the orders
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Multiple
      - Orders
      - In
      - Database
      - ""
      - "No"
      - URL
      - Parameters
      - Should
      - Be
      - Included
    post:
      summary: Adds a new order to the system
      description: Adds a new order to the system.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1orders-post
      parameters:
      - in: query
        name: bypassorderemail
        description: will bypass sending the customer new order email if normally
          applicable
      - in: query
        name: bypassorderprocessing
        description: will bypass/ignore stock updates, gift certificates generation,
          rewards, etc
      - in: body
        name: order
        description: A Json or XML object containing the new order
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Order
      - To
      - System
    get:
      summary: ""
      description: .
      operationId: Orders_GetAllOrders
      x-api-path-slug: 3dcartwebapiv1orders-get
      parameters:
      - in: query
        name: billingemail
      - in: query
        name: countonly
      - in: query
        name: dateend
      - in: query
        name: datestart
      - in: query
        name: invoicenumber
      - in: query
        name: invoicenumberend
      - in: query
        name: invoicenumberstart
      - in: query
        name: invoiceprefix
      - in: query
        name: lastupdateend
      - in: query
        name: lastupdatestart
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: orderstatus
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - ""
  /3dCartWebAPI/v1/Orders/{orderid}:
    get:
      summary: Get a specific order
      description: Get a specific order.
      operationId: Orders_GetOrder
      x-api-path-slug: 3dcartwebapiv1ordersorderid-get
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Order
    put:
      summary: This method is used to update a single order record in the database.
        The {orderid} parameter specifies which order record to update.
      description: This method is used to update a single order record in the database.
        the {orderid} parameter specifies which order record to update..
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderid-put
      parameters:
      - in: body
        name: order
        description: A Json or XML object containing the order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Order
      - Record
      - In
      - Database
      - ""
      - Orderid
      - Parameter
      - Specifies
      - Which
      - Order
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/Orders/{orderid}/Items:
    get:
      summary: Gets the items from a specific Order
      description: Gets the items from a specific order.
      operationId: Orders_GetAllOrderItems
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Items
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of items from a specific Order
      description: Updates a collection of items from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-put
      parameters:
      - in: body
        name: items
        description: A Json or XML object containing the new items
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Items
      - From
      - Specific
      - Order
    post:
      summary: Adds a new item on the order
      description: Adds a new item on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderiditems-post
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Item
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Questions:
    get:
      summary: Gets the questions from a specific Order
      description: Gets the questions from a specific order.
      operationId: Orders_GetAllOrderQuestions
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Questions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of questions from a specific Order
      description: Updates a collection of questions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: questions
        description: A Json or XML object containing the new questions
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Questions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new question on the order
      description: Adds a new question on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Question
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments:
    get:
      summary: Gets the shipments from a specific Order
      description: Gets the shipments from a specific order.
      operationId: Orders_GetAllOrderShipments
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Shipments
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of shipments from a specific Order
      description: Updates a collection of shipments from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipments
        description: A Json or XML object containing the new shipments
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Shipments
      - From
      - Specific
      - Order
    post:
      summary: Adds a new shipment on the order
      description: Adds a new shipment on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipments-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipment
        description: A Json or XML object containing the new shipment
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Shipment
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Shipments/{shipmentid}:
    put:
      summary: Updates a specific shipment from a specific Order
      description: Updates a specific shipment from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidshipmentsshipmentid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: body
        name: shipment
        description: A Json or XML object containing the new shipment
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: shipmentid
        description: ShipmentID
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Shipment
      - From
      - Specific
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions:
    get:
      summary: Gets the transactions from a specific Order
      description: Gets the transactions from a specific order.
      operationId: Orders_GetAllOrderTransactions
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Transactions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of transactions from a specific Order
      description: Updates a collection of transactions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transactions
        description: A Json or XML object containing the new transactions
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Transactions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new transaction on the order
      description: Adds a new transaction on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Transaction
      - "On"
      - Order
  /3dCartWebAPI/v1/Cart/{orderkey}:
    put:
      summary: This method is used to update a single cart record in the database.
        The {orderkey} parameter specifies which cart record to update.
      description: This method is used to update a single cart record in the database.
        the {orderkey} parameter specifies which cart record to update..
      operationId: Carts_Update
      x-api-path-slug: 3dcartwebapiv1cartorderkey-put
      parameters:
      - in: body
        name: cart
        description: A Json or XML object containing the cart
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderkey
        description: Order Key
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Update
      - Single
      - Cart
      - Record
      - In
      - Database
      - ""
      - Orderkey
      - Parameter
      - Specifies
      - Which
      - Cart
      - Record
      - To
      - Update
  /3dCartWebAPI/v1/OrderStatus:
    get:
      summary: Get all OrderStatus
      description: Get all orderstatus.
      operationId: OrderStatus_GetAllOrderStatus
      x-api-path-slug: 3dcartwebapiv1orderstatus-get
      parameters:
      - in: query
        name: countonly
        description: Count the number of rows only
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - OrderStatus
  /3dCartWebAPI/v1/OrderStatus/{id}:
    get:
      summary: Get an OrderStatus
      description: Get an orderstatus.
      operationId: OrderStatus_GetOrderStatus
      x-api-path-slug: 3dcartwebapiv1orderstatusid-get
      parameters:
      - in: path
        name: id
        description: OrderStatus ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - OrderStatus
  /3dCartWebAPI/v1/Orders/{orderid}/Items/{itemindexid}:
    put:
      summary: Updates a specific item from a specific Product
      description: Updates a specific item from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderiditemsitemindexid-put
      parameters:
      - in: body
        name: item
        description: A Json or XML object containing the new item
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: itemindexid
        description: The unique indexID of an Item
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Item
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Orders/{orderid}/Questions/{questionanswerindexid}:
    put:
      summary: Updates a specific question from a specific Product
      description: Updates a specific question from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestionsquestionanswerindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: questionanswerindexid
        description: QuestionID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Question
      - From
      - Specific
      - Product
  /3dCartWebAPI/v1/Orders/{orderid}/Transactions/{transactionindexid}:
    put:
      summary: Updates a specific transaction from a specific Product
      description: Updates a specific transaction from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidtransactionstransactionindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      - in: body
        name: transaction
        description: A Json or XML object containing the new transaction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: transactionindexid
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Transaction
      - From
      - Specific
      - Product
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