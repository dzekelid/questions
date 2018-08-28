---
swagger: "2.0"
x-collection-name: Okta
x-complete: 0
info:
  title: Okta Change Recovery Question
  description: Change recovery question.
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}/credentials/change_recovery_question:
    post:
      summary: Change Recovery Question
      description: Change recovery question.
      operationId: postUsersUserCredentialsChangeRecoveryQuestion
      x-api-path-slug: usersuseridcredentialschange-recovery-question-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Change
      - Recovery
      - Question
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