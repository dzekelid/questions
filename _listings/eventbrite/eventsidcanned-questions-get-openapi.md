---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Events Canned Questions
  description: 'This endpoint returns canned questions of a single event (examples:
    first name, last name, company, prefix, etc.). This endpoint will return question.'
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/canned_questions/:
    get:
      summary: Get Events Canned Questions
      description: 'This endpoint returns canned questions of a single event (examples:
        first name, last name, company, prefix, etc.). This endpoint will return question.'
      operationId: getEventsCannedQuestions
      x-api-path-slug: eventsidcanned-questions-get
      parameters:
      - in: query
        name: as_owner
        description: Return private events and more details
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Canned
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