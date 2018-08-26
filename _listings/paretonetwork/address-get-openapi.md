---
swagger: "2.0"
x-collection-name: ParetoNetwork
x-complete: 0
info:
  title: Pareto Get the information of the current user
  description: Get the information of the current user. The current user is fetched
    using the auth cookie.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sign:
    post:
      summary: Cookie authentication
      description: Test the hash between a message and public key. If the test is
        passed, a cookie is stored. The parameters of this request are gotten from
        MetaMask
      operationId: postSign
      x-api-path-slug: sign-post
      responses:
        200:
          description: OK
      tags:
      - Sign
  /rank:
    get:
      summary: Get the list of all addresses sorted by rank
      description: Get all the addresses sorted by rank. The ranking is gotten from
        the Ethereum score
      operationId: getRank
      x-api-path-slug: rank-get
      responses:
        200:
          description: OK
      tags:
      - Rank
  /auth:
    get:
      summary: Test if user is properly authenticated
      description: Simple authenticated method to determine if user is properly authenticated.
      operationId: getAuth
      x-api-path-slug: auth-get
      responses:
        200:
          description: OK
      tags:
      - Auth
  /unsign:
    post:
      summary: Unsign http client for the current user
      description: Manage unsign proccess. Delete cookie with header set-cookie
      operationId: postUnsign
      x-api-path-slug: unsign-post
      responses:
        200:
          description: OK
      tags:
      - Unsign
  /address:
    get:
      summary: Get the information of the current user
      description: Get the information of the current user. The current user is fetched
        using the auth cookie.
      operationId: getAddress
      x-api-path-slug: address-get
      responses:
        200:
          description: OK
      tags:
      - Address
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