swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/saveadditionalquestions:
    put:
      summary: To edit the Group additional questions
      description: To edit the group additional questions.
      operationId: Group_SaveAdditionalQuestionsByidByadditionalQuestions
      x-api-path-slug: apigroupidsaveadditionalquestions-put
      parameters:
      - in: body
        name: additionalQuestions
        description: The additional questions to set on the group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The group id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Edit
      - Group
      - Additional
      - Questions