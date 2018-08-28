swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions:
    get:
      summary: Get attendee questions
      description: Get attendee questions.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyQuestionsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
      - Questions
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/questions:
    get:
      summary: Get session questions
      description: Get session questions.
      operationId: WebinarsSessionsSessionKeyQuestionsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyquestions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Session
      - Questions