{
  "info": {
    "name": "Pareto Update the profile of the current user",
    "_postman_id": "eec84373-abdc-4e2c-8221-f2fb7b4ef4ff",
    "description": "Update the profile of the current user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "733591f8-25b5-488b-85d6-2c3c09ff96f1",
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
              "id": "d9d84f07-113a-4307-af5c-94fca0aa02ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Rank",
      "item": [
        {
          "id": "671b96a4-1299-4ee2-b288-0b69b7a36831",
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
              "id": "e465280d-5ab7-4d04-bbc3-3c989f6b4031"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "5c42bf4b-768c-452a-beb0-c19af12b8fa9",
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
              "id": "2dd3c5b7-deb2-4a21-b5db-abe9ed690f25"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsign",
      "item": [
        {
          "id": "fc5b6543-bcb5-4995-a355-b77726e2b6c0",
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
              "id": "4b584884-d307-4e84-b570-3693f57f27ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "660bf282-3177-4299-beab-e4cacda88bec",
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
              "id": "b36b2514-3c08-4994-bbce-81e694519a9e"
            }
          ]
        },
        {
          "id": "ab7da36a-54ac-4c4d-a509-3bd670b23115",
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
              "id": "df450e40-0148-45be-a96e-3983a1888263"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "6e5cd830-6da4-4352-808c-7adc5376889b",
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
              "id": "74f47257-7f2c-4d8a-a0e8-8ab1d4dda727"
            }
          ]
        },
        {
          "id": "a2b0ac28-4304-4e0b-9cc9-84e2adbbee4f",
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
              "id": "bd875124-f96a-4849-ba5d-7cfc54a36d2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Userinfo",
      "item": [
        {
          "id": "53165335-b6ef-486c-9cce-c0f243610fa1",
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
              "id": "db6b1bf0-fd73-4dd9-9982-2bc8c1db87f6"
            }
          ]
        },
        {
          "id": "cfbabf13-9626-4d67-9c43-d6fe49d22d92",
          "name": "getUserinfoAddress",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "userinfo/:address"
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
            "description": "Get the profile of a specific user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e64c4438-bc5f-4607-b52d-bb80eb14e64c"
            }
          ]
        }
      ]
    },
    {
      "name": "Updateuser",
      "item": [
        {
          "id": "2ec9218d-e493-46ac-9781-e2385a8b7b07",
          "name": "postUpdateuser",
          "request": {
            "url": "{{default}}/updateuser",
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
            "description": "Update the profile of the current user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c2736c5-379b-498a-82fe-2d6916cec6fa"
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