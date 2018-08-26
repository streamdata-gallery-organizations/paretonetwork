{
  "info": {
    "name": "Pareto Get the content available for current user",
    "_postman_id": "f83d2933-d2b5-4492-a6c1-b247ab44dda2",
    "description": "Get the content available for current user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "310ef667-94f1-43b4-9cdf-fad6fb7527d0",
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
              "id": "77c4f9d2-c308-468f-b52d-8049fcd06360"
            }
          ]
        }
      ]
    },
    {
      "name": "Rank",
      "item": [
        {
          "id": "812747d9-92b6-4f6c-9bce-221ac9f987cb",
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
              "id": "cbd3345d-2f63-4e52-8f26-88b989f7180d"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "1669be66-c6aa-4852-9625-409e822e99aa",
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
              "id": "6791403e-7c8f-48a7-8c52-eefafd93deab"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsign",
      "item": [
        {
          "id": "247a0ccb-e40b-4abe-9810-61994ca25e6d",
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
              "id": "94d0467b-a1a8-4d2d-a040-e11ee4f3755e"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "4ce3031d-e0c7-483e-9905-971739aba725",
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
              "id": "59c7f1d2-5002-4cf8-ac3b-6cf4f030783c"
            }
          ]
        },
        {
          "id": "f9a5afd4-1023-4c60-b089-bba6fba2f813",
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
              "id": "e1068fb6-4c0c-4445-ad6f-1b7dcfa37d39"
            }
          ]
        }
      ]
    },
    {
      "name": "Content",
      "item": [
        {
          "id": "8630e2a3-5579-49ad-93c9-4689c49079ae",
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
              "id": "be6a121f-4c21-4c36-b627-2b4cc02db7a1"
            }
          ]
        },
        {
          "id": "97404a25-0e07-4617-9622-3419538dd6e0",
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
              "id": "ba1d50ec-1dee-458e-8f3f-3c34cf7c47e3"
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