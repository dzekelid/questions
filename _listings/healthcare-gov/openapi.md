---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 1
info:
  title: Healthcare
  version: 1.0.0
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
---