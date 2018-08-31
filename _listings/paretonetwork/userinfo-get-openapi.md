---
swagger: "2.0"
x-collection-name: ParetoNetwork
x-complete: 0
info:
  title: Pareto Get the information of the profile user
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
  /address/{address}:
    get:
      summary: Get the information of a specific user
      description: Get the information of a specific user.
      operationId: getAddressAddress
      x-api-path-slug: addressaddress-get
      parameters:
      - in: path
        name: address
        description: address to use
      responses:
        200:
          description: OK
      tags:
      - Address
      - Address
  /content:
    get:
      summary: Get the content about the actionable investing intels
      description: Get all available content about the actionable investing intels.
      operationId: getContent
      x-api-path-slug: content-get
      responses:
        200:
          description: OK
      tags:
      - Content
  /content/me:
    get:
      summary: Get the content available for current user
      description: Get the content available for current user
      operationId: getContentMe
      x-api-path-slug: contentme-get
      responses:
        200:
          description: OK
      tags:
      - Content
      - Me
  /userinfo:
    get:
      summary: Get the information of the profile user
      description: Get the information of the current user. The current user is fetched
        using the auth cookie.
      operationId: getUserinfo
      x-api-path-slug: userinfo-get
      parameters:
      - in: query
        name: latest
        description: if true force update ranking
      responses:
        200:
          description: OK
      tags:
      - Userinfo
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