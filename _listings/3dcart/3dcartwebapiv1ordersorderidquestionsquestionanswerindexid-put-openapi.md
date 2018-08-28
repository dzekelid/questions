---
swagger: "2.0"
x-collection-name: 3dcart
x-complete: 0
info:
  title: 3dcart Updates a specific question from a specific Product
  version: 1.0.0
  description: Updates a specific question from a specific product.
host: apirest.3dcart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3dCartWebAPI/v1/Orders/{orderid}/Questions:
    get:
      summary: Gets the questions from a specific Order
      description: Gets the questions from a specific order.
      operationId: Orders_GetAllOrderQuestions
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of items that can be returned
      - in: query
        name: offset
        description: Starting point for the return data
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Questions
      - From
      - Specific
      - Order
    put:
      summary: Updates a collection of questions from a specific Order
      description: Updates a collection of questions from a specific order.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: questions
        description: A Json or XML object containing the new questions
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Collection
      - Of
      - Questions
      - From
      - Specific
      - Order
    post:
      summary: Adds a new question on the order
      description: Adds a new question on the order.
      operationId: Orders_Post
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestions-post
      parameters:
      - in: path
        name: orderid
        description: Order ID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - New
      - Question
      - "On"
      - Order
  /3dCartWebAPI/v1/Orders/{orderid}/Questions/{questionanswerindexid}:
    put:
      summary: Updates a specific question from a specific Product
      description: Updates a specific question from a specific product.
      operationId: Orders_Update
      x-api-path-slug: 3dcartwebapiv1ordersorderidquestionsquestionanswerindexid-put
      parameters:
      - in: path
        name: orderid
        description: OrderID
      - in: header
        name: PrivateKey
        description: PrivateKey
      - in: body
        name: question
        description: A Json or XML object containing the new question
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: questionanswerindexid
        description: QuestionID
      - in: header
        name: SecureURL
        description: SecureURL
      - in: header
        name: Token
        description: Token
      responses:
        200:
          description: OK
      tags:
      - S
      - Specific
      - Question
      - From
      - Specific
      - Product
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