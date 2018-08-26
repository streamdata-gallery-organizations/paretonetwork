{
  "info": {
    "name": "Pareto Get the information of a specific user",
    "_postman_id": "bb5cac04-31c6-4db0-9904-d9cf171fa892",
    "description": "Get the information of a specific user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "1cbcb860-c929-4882-bc39-a6b88ad3d132",
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
              "id": "204ff36a-1a9e-4a70-9008-094cdaeecbd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Rank",
      "item": [
        {
          "id": "0c06e2ea-f32b-4196-ac74-55d65ac33f93",
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
              "id": "f9828ed1-b8bd-4c3c-9734-e672e43a86aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Auth",
      "item": [
        {
          "id": "57f797ff-56d0-4682-809c-4d8287ecd070",
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
              "id": "32e6840f-08f6-471c-9ada-93b339103c8f"
            }
          ]
        }
      ]
    },
    {
      "name": "Unsign",
      "item": [
        {
          "id": "08d13757-5ae5-4a46-add8-21b1b84f9963",
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
              "id": "132406fd-7e72-4a4a-9248-e5708b2bb527"
            }
          ]
        }
      ]
    },
    {
      "name": "Address",
      "item": [
        {
          "id": "3a8b2a97-1925-49af-a1a6-111c1653c256",
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
              "id": "395081b9-84b6-4cbc-bda2-b3210a595864"
            }
          ]
        },
        {
          "id": "1d78b5b5-47b8-4af9-9254-0705ef635e98",
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
              "id": "45af221b-4168-4e67-ba29-e977ab02dff7"
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