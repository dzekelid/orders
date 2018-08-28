{
  "info": {
    "name": "Open Bank Project Get Account Standing Orders",
    "_postman_id": "74a483d0-561d-454b-9c53-803d1e19a960",
    "description": "Get Standing Orders related to an account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Banking",
      "item": [
        {
          "id": "3847133a-dc94-486e-914a-0f5f7821ad50",
          "name": "CreateAccountRequest",
          "request": {
            "url": "{{default}}/account-requests?No Name=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d52d913-baf6-40fe-8a12-98bedd0c2f70"
            }
          ]
        },
        {
          "id": "0d955b4e-3440-4d4d-aacc-c56c9eb76df1",
          "name": "GetAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b45a6bb8-eaec-4481-841f-b5f621993b9d"
            }
          ]
        },
        {
          "id": "fc5f0783-880d-4c23-ab41-81754b751e20",
          "name": "DeleteAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f16d4dfc-61cb-46bb-b89b-7037735aff69"
            }
          ]
        },
        {
          "id": "3504b2bb-4ca2-40fd-a352-a0bf47df1261",
          "name": "GetAccounts",
          "request": {
            "url": "{{default}}/accounts?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8c206af-88fe-4591-b210-1130808dbb1a"
            }
          ]
        },
        {
          "id": "0e3dd513-99c8-4a64-befd-ae16ccee6aab",
          "name": "GetAccount",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b87787d-51a0-4ac4-8850-e04684b74fa5"
            }
          ]
        },
        {
          "id": "b798ed43-00c1-4077-b429-7d10092d41e3",
          "name": "GetAccountTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efc7acdf-7c3b-4d91-9d99-e1c35cf0ca76"
            }
          ]
        },
        {
          "id": "1266cdba-2964-42b6-b7b8-3d12192924b3",
          "name": "GetAccountBeneficiaries",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/beneficiaries"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04e8dbf3-3471-4fa1-a57c-f0dea23241ff"
            }
          ]
        },
        {
          "id": "b125fe67-c45d-4d9a-860f-9849ded8b4c2",
          "name": "GetAccountBalances",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/balances"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98b59e00-3601-4e0b-9330-c7d169e33639"
            }
          ]
        },
        {
          "id": "716cb1ea-83e5-4eeb-afd0-99e683144a57",
          "name": "GetAccountDirectDebits",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/direct-debits"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1746baf3-0c97-41e8-85d2-06c990aadc41"
            }
          ]
        },
        {
          "id": "233656cb-43a0-4216-8440-f6b08ae3c943",
          "name": "GetAccountStandingOrders",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/standing-orders"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6dd79ea-ecc8-4365-82c6-32ec07da4148"
            }
          ]
        },
        {
          "id": "dd2c3559-fd9e-45c7-a8c5-c645ef4df8ee",
          "name": "GetAccountProduct",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/product"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Product related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3078c521-8a67-423d-a6b5-4ad9a5180b05"
            }
          ]
        },
        {
          "id": "8273c1fe-694f-4c6b-855c-214278fc39b8",
          "name": "GetAccountOffers",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/offers"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fec9e31-d308-45e4-838f-466083497f57"
            }
          ]
        },
        {
          "id": "4422eb4b-9152-4afa-964d-5672e32fcffa",
          "name": "GetAccountParty",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/party"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df51df11-2f94-4608-b548-152e90b5958d"
            }
          ]
        },
        {
          "id": "074ede84-5b07-40ac-ae02-dc4685430d94",
          "name": "GetAccountScheduledPayments",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/scheduled-payments"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e604042d-1f74-4f47-8e7c-2d1f71778b9f"
            }
          ]
        },
        {
          "id": "67df004a-c21b-40ed-acba-6808135f4678",
          "name": "GetAccountStatements",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a87fffbc-9189-453a-bc1b-7eef46bd2a96"
            }
          ]
        },
        {
          "id": "c0d019d1-19be-4576-beed-8c747487b53d",
          "name": "GetAccountStatement",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "486b14ef-43ec-4a6e-b933-41e921ff0176"
            }
          ]
        },
        {
          "id": "1cb9a875-65b1-4e3b-b03d-be368d6e49c4",
          "name": "GetAccountStatementFile",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/file"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement File related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a012a61e-731e-4ece-83d6-ea90c27a7c39"
            }
          ]
        },
        {
          "id": "7588f7e0-938c-41af-8ff5-e78e2509bb96",
          "name": "GetAccountStatementTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement Transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6466b5ea-454d-4133-83b1-9763e427bbbc"
            }
          ]
        },
        {
          "id": "1d6c7b8f-220e-421d-86b0-9532087d40b6",
          "name": "GetStandingOrders",
          "request": {
            "url": "{{default}}/standing-orders?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05cc2439-ffda-4d72-b73c-263f55bf724f"
            }
          ]
        },
        {
          "id": "8d979134-cb6e-4755-a614-ed424e5f1ef7",
          "name": "GetDirectDebits",
          "request": {
            "url": "{{default}}/direct-debits?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e66bd1ce-2c5a-4d5a-bc72-0312c03075b0"
            }
          ]
        },
        {
          "id": "4a48a25a-8f01-4012-b6d2-f843832c1bc0",
          "name": "GetBeneficiaries",
          "request": {
            "url": "{{default}}/beneficiaries?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b3fbc51-0644-444d-9c1a-031b04edabf7"
            }
          ]
        },
        {
          "id": "ac565793-8ae4-49ce-bdaf-1696b0dd54a7",
          "name": "GetTransactions",
          "request": {
            "url": "{{default}}/transactions?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bad4bdbe-c413-4971-8e03-9f4eb77a01b3"
            }
          ]
        },
        {
          "id": "9989191c-8cf2-4cfb-93bf-772832c1df82",
          "name": "GetBalances",
          "request": {
            "url": "{{default}}/balances?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76ff4cae-6143-4e64-b6d4-02d56098aeb9"
            }
          ]
        },
        {
          "id": "bb2f206d-e407-4665-b6ac-53087ea7b8af",
          "name": "GetProducts",
          "request": {
            "url": "{{default}}/products?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Products"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4be5e3ee-6c5a-4137-8e25-146fa1257319"
            }
          ]
        },
        {
          "id": "23c39d6d-8823-49ed-8f1d-926d370495e3",
          "name": "GetOffers",
          "request": {
            "url": "{{default}}/offers?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc90b724-8985-431c-8ea1-b99653895d86"
            }
          ]
        },
        {
          "id": "4b3cc1f3-935a-4262-a10a-ac5f2ec26aad",
          "name": "GetParty",
          "request": {
            "url": "{{default}}/party?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcac2ba4-bf31-4c6a-91dc-c559be0ddb0d"
            }
          ]
        },
        {
          "id": "c635186c-b9f6-4715-b986-284b8f27b48a",
          "name": "GetScheduledPayments",
          "request": {
            "url": "{{default}}/scheduled-payments?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "076dfbe0-a8dc-4cbb-82a3-c6717fd65f6f"
            }
          ]
        },
        {
          "id": "fc514c4a-f410-4222-9ecf-db1531125e38",
          "name": "GetStatements",
          "request": {
            "url": "{{default}}/statements?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dae470c7-b5b2-4050-8f18-381d79df1a73"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/open-banking/v2.0"
    }
  ]
}