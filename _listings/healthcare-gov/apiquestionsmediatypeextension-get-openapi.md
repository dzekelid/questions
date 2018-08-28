---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 0
info:
  title: HealthCare.gov Get Questions
  version: 1.0.0
  description: Returns pages content.
host: www.healthcare.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/questions{mediaTypeExtension}:
    get:
      summary: Get Questions
      description: Returns pages content.
      operationId: getApiQuestionsMediatypeextension
      x-api-path-slug: apiquestionsmediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      responses:
        200:
          description: OK
      tags:
      - Questions
  /es/question/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Question Pagename
      description: Returns pages content.
      operationId: getEsQuestionPagenameMediatypeextension
      x-api-path-slug: esquestionpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Question
      - Pagename
  /question/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Question Pagename
      description: Returns pages content.
      operationId: getQuestionPagenameMediatypeextension
      x-api-path-slug: questionpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Question
      - Pagename
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