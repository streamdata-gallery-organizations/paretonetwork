{
  "info": {
    "name": "Pareto Cookie authentication",
    "_postman_id": "99d9f1c8-9623-46a7-bb7f-8a65802f1aed",
    "description": "Test the hash between a message and public key. If the test is passed, a cookie is stored. The parameters of this request are gotten from MetaMask",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sign",
      "item": [
        {
          "id": "c09caf70-c3c3-4f74-b69e-544cc3d85d98",
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
              "id": "264e66ed-0988-4592-b034-5660f02fc3cf"
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