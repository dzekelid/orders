{
  "info": {
    "name": "Steem get_open_orders",
    "_postman_id": "c4b1a0de-8ee0-434a-99b0-ad56894f1bef",
    "description": "get_open_orders",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "9a31713d-d541-47e0-ace8-5b27616013eb",
          "name": "returns-version-information-of-connected-steem-nodewebsocket",
          "request": {
            "url": "http://api.steemjs.com/get_version",
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
            "description": "Returns version information of connected Steem node/websocket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0122583-288c-4e80-8bc1-cadc7a1a9776"
            }
          ]
        },
        {
          "id": "bd6a710c-c6bc-4189-9c0d-022c610afd2d",
          "name": "get-chain-properties",
          "request": {
            "url": "http://api.steemjs.com/get_chain_properties",
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
            "description": "get chain properties"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "030780c2-0620-4180-b28d-a4ccd83bb1df"
            }
          ]
        },
        {
          "id": "53c0dfce-a598-41d7-b6cd-545fac178425",
          "name": "get-config",
          "request": {
            "url": "http://api.steemjs.com/get_config",
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
            "description": "get config"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1d03984-ce5a-49c8-9276-174e4ed6381f"
            }
          ]
        },
        {
          "id": "f3dc9318-94b7-4219-9432-f7991311fea3",
          "name": "get-dynamic-global-properties",
          "request": {
            "url": "http://api.steemjs.com/get_dynamic_global_properties",
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
            "description": "get_dynamic_global_properties"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ec735d4-ac7c-4cbc-a201-e90f3a119e96"
            }
          ]
        },
        {
          "id": "c3911069-769c-42c9-a263-ea5b96fb09ef",
          "name": "get-feed-history",
          "request": {
            "url": "http://api.steemjs.com/get_feed_history",
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
            "description": "get_feed_history"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8732fb95-2bc9-4fc5-b972-de9f794f47ea"
            }
          ]
        },
        {
          "id": "b0d7fd4d-3cfd-4cf0-8bbd-2d2892d30806",
          "name": "get-current-median-history-price",
          "request": {
            "url": "http://api.steemjs.com/get_current_median_history_price",
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
            "description": "get_current_median_history_price"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed0f3eb1-5472-48e3-9b81-b7ed0b2d43d0"
            }
          ]
        },
        {
          "id": "5118b846-7a4e-47e0-a752-0aa7a4012788",
          "name": "get-hardfork-version",
          "request": {
            "url": "http://api.steemjs.com/get_hardfork_version",
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
            "description": "get_hardfork_version"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e22906e4-2df2-466e-b8d0-5e3c92df51a8"
            }
          ]
        },
        {
          "id": "1008156f-da8c-4934-b516-175f0ce8637a",
          "name": "get-next-scheduled-hardfork",
          "request": {
            "url": "http://api.steemjs.com/get_next_scheduled_hardfork",
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
            "description": "get_next_scheduled_hardfork"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee8161bd-dd96-4928-bae9-bc1287924e55"
            }
          ]
        },
        {
          "id": "f82ba20b-83d5-4758-8bdf-ba714121c915",
          "name": "get-witness-count",
          "request": {
            "url": "http://api.steemjs.com/get_witness_count",
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
            "description": "get_witness_count"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6674378d-be74-4065-850f-5b0e3bbbca15"
            }
          ]
        },
        {
          "id": "5b8aa9a2-9446-4f64-a5fb-a93c7f56726e",
          "name": "get-witness-schedule",
          "request": {
            "url": "http://api.steemjs.com/get_witness_schedule",
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
            "description": "get_witness_schedule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b66e5d3-ffe6-4004-b962-6680f81db0bc"
            }
          ]
        },
        {
          "id": "17d908ef-a70f-4ea3-a064-fdabb56aec2a",
          "name": "get-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses?witnessIds=%7B%7D",
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
            "description": "get_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08d5fda2-a0d6-40f3-a07a-00910ac00247"
            }
          ]
        },
        {
          "id": "db206ec5-d0b1-4ff6-a62c-94cae99e68f7",
          "name": "get-witness-by-account",
          "request": {
            "url": "http://api.steemjs.com/get_witness_by_account?accountName=%7B%7D",
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
            "description": "get_witness_by_account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2aeb7711-bbde-4255-bc8a-8449132bb4c5"
            }
          ]
        },
        {
          "id": "a2614fb1-a5e7-493b-8221-0a1086a39281",
          "name": "get-witnesses-by-vote",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses_by_vote?from=%7B%7D&limit=%7B%7D",
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
            "description": "get_witnesses_by_vote"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb2fff97-d87e-462c-bbc4-6d00053a1b40"
            }
          ]
        },
        {
          "id": "74e5fa2d-1072-415b-b195-4b8c3f1171e5",
          "name": "get-active-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_active_witnesses",
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
            "description": "get_active_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e457dfd8-e39c-4b3f-8eb5-2f990c8aca5f"
            }
          ]
        },
        {
          "id": "a01518f0-0af3-4f02-843f-cb73c6069016",
          "name": "get-miner-queue",
          "request": {
            "url": "http://api.steemjs.com/get_miner_queue",
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
            "description": "get_miner_queue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3972e173-c32c-47d2-a1d9-88131a76ea85"
            }
          ]
        },
        {
          "id": "b3ff049d-cc0d-458a-8a3f-ded4872aff69",
          "name": "get-liquidity-queue",
          "request": {
            "url": "http://api.steemjs.com/get_liquidity_queue?limit=%7B%7D&startAccount=%7B%7D",
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
            "description": "get_liquidity_queue"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c0f9ce1d-9d21-40cf-9f6b-ddd26c7151ba"
            }
          ]
        },
        {
          "id": "a026a08d-6d3c-4cf3-a3ec-577894c321ff",
          "name": "get-open-orders",
          "request": {
            "url": "http://api.steemjs.com/get_open_orders?owner=%7B%7D",
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
            "description": "get_open_orders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d496bb68-70e6-45c2-b677-973c78ec3aca"
            }
          ]
        }
      ]
    },
    {
      "name": "Number",
      "item": [
        {
          "id": "949f9771-75f0-4c04-aedf-2e4239db6b9d",
          "name": "get-number-of-accounts-from-steem",
          "request": {
            "url": "http://api.steemjs.com/get_account_count",
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
            "description": "Get Number of Accounts from Steem"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a95c74cb-92db-491f-a2ca-9fd6c7583ddd"
            }
          ]
        }
      ]
    },
    {
      "name": "Lookup",
      "item": [
        {
          "id": "499e5eb0-776d-4c82-92e0-db56fe887076",
          "name": "lookup-witness-accounts-regex-search",
          "request": {
            "url": "http://api.steemjs.com/lookup_witness_accounts?limit=%7B%7D&lowerBoundName=%7B%7D",
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
            "description": "lookup_witness_accounts regex search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9dd26904-a8f3-4f9a-a1cb-cc1888271256"
            }
          ]
        }
      ]
    },
    {
      "name": "Witness",
      "item": [
        {
          "id": "857f0bbc-9cb7-4d4f-96e1-6daf9ecffa4c",
          "name": "witness-update",
          "request": {
            "url": "http://api.steemjs.com/witness_update?block_signing_key=%7B%7D&fee=%7B%7D&owner=%7B%7D&props=%7B%7D&url=%7B%7D",
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
            "description": "witness_update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ade86ad1-b574-4095-9e6c-a6bec886b3d2"
            }
          ]
        }
      ]
    }
  ]
}