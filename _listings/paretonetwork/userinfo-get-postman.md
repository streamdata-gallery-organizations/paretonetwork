{
  "info": {
    "name": "Pareto Get the information of the profile user",
    "_postman_id": "261881be-8606-4cf9-8c6f-ccd151e5674b",
    "description": "Get the information of the current user. The current user is fetched using the auth cookie.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "aa2c982b-c9ae-49f4-bd35-43735bca74fd",
          "name": "postSign",
          "request": {
            "url": "{{default}}/sign",
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
            "description": "Test the hash between a message and public key. If the test is passed, a cookie is stored. The parameters of this request are gotten from MetaMask"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2c8f0d7-7738-4e8f-99ed-f80e4b7f23c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Rank",
      "item": [
        {
          "id": "ecc7c59d-1fa6-4000-9197-62542bf0ef37",
          "name": "getRank",
          "request": {
            "url": "{{default}}/rank",
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
            "description": "Get all the addresses sorted by rank. The ranking is gotten from the Ethereum score"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c7ca8b5-9b73-4879-9c50-6e5625ad7ba3"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "58c96369-d850-440a-9d90-61573a578fed",
          "name": "getAuth",
          "request": {
            "url": "{{default}}/auth",
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
            "description": "Simple authenticated method to determine if user is properly authenticated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f145b687-79e0-41cf-87d2-640418d2273b"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsign",
      "item": [
        {
          "id": "36689087-7abd-4260-a327-dd0814183683",
          "name": "postUnsign",
          "request": {
            "url": "{{default}}/unsign",
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
            "description": "Manage unsign proccess. Delete cookie with header set-cookie"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b3473f3-f586-44c5-a528-c972d95044be"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "0e522145-d3c7-4849-8f18-a0d897d7a98f",
          "name": "getAddress",
          "request": {
            "url": "{{default}}/address",
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
            "description": "Get the information of the current user. The current user is fetched using the auth cookie."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14d0d9a3-d73c-4440-8906-fab687d11d5c"
            }
          ]
        },
        {
          "id": "79dc1ea8-d5a8-4d64-b8d1-76b52d790a45",
          "name": "getAddressAddress",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "address/:address"
              ],
              "variable": [
                {
                  "id": "address",
                  "value": "{}",
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
            "description": "Get the information of a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c15a9c5-b1e3-42ec-857f-c7df35366f80"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "e6e77e58-c5de-4cb3-97bd-9c52a92cecc1",
          "name": "getContent",
          "request": {
            "url": "{{default}}/content",
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
            "description": "Get all available content about the actionable investing intels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb390b88-0d7f-43f2-b631-abba261875f7"
            }
          ]
        },
        {
          "id": "78689c28-9439-4347-9feb-14ac601a04a6",
          "name": "getContentMe",
          "request": {
            "url": "{{default}}/content/me",
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
            "description": "Get the content available for current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28ea4bf7-ecc7-4647-b6ce-a5b380f2c0f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Userinfo",
      "item": [
        {
          "id": "a697128c-9ead-4e27-9fcd-bef796276fd9",
          "name": "getUserinfo",
          "request": {
            "url": "{{default}}/userinfo?latest=%7B%7D",
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
            "description": "Get the information of the current user. The current user is fetched using the auth cookie."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beceb90d-0320-4409-a7ca-f67e180ab899"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/"
    }
  ]
}