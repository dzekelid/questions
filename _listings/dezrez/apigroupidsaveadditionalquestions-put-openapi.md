---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez To edit the Group additional questions
  version: 1.0.0
  description: To edit the group additional questions.
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