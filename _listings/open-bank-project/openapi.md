swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/standing-orders:
    get:
      summary: Get Account Standing Orders
      description: Get Standing Orders related to an account
      operationId: GetAccountStandingOrders
      x-api-path-slug: accountsaccountidstandingorders-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Standing
      - Orders
  /standing-orders:
    get:
      summary: Get Standing Orders
      description: Get Standing Orders
      operationId: GetStandingOrders
      x-api-path-slug: standingorders-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Standing
      - Orders