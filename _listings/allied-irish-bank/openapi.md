---
swagger: "2.0"
x-collection-name: Allied Irish Bank
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v1.1
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
      - in: path
        name: AccountId
        description: A unique identifier used to identify the account resource
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
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
      - in: header
        name: Authorization
        description: An Authorisation Token as per https://tools
      - in: header
        name: x-fapi-customer-ip-address
        description: The PSUs IP address if the PSU is currently logged in with the
          TPP
      - in: header
        name: x-fapi-customer-last-logged-time
        description: The time when the PSU last logged in with the TPP
      - in: header
        name: x-fapi-financial-id
        description: The unique id of the ASPSP to which the request is issued
      - in: header
        name: x-fapi-interaction-id
        description: An RFC4122 UID used as a correlation id
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Standing
      - Orders
---