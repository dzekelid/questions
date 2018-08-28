---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List questions in a quiz or a submission
  description: List questions in a quiz or a submission.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/quizzes/quiz_id/questions:
    get:
      summary: List questions in a quiz or a submission
      description: List questions in a quiz or a submission.
      operationId: list-questions-in-a-quiz-or-a-submission
      x-api-path-slug: coursescourse-idquizzesquiz-idquestions-get
      parameters:
      - in: query
        name: quiz_submission_attempt
        description: The attempt of the submission you want the questions for
      - in: query
        name: quiz_submission_id
        description: If specified, the endpoint will return the questions that were
          presentednfor that submission
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
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