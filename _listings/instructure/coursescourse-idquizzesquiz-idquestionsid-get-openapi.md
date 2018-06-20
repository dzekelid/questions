---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Get a single quiz question
  description: Get a single quiz question.
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
    post:
      summary: Create a single quiz question
      description: Create a single quiz question.
      operationId: create-a-single-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestions-post
      parameters:
      - in: query
        name: question[answers]
        description: no description
      - in: query
        name: question[correct_comments]
        description: The comment to display if the student answers the question correctly
      - in: query
        name: question[incorrect_comments]
        description: The comment to display if the student answers incorrectly
      - in: query
        name: question[neutral_comments]
        description: The comment to display regardless of how the student answered
      - in: query
        name: question[points_possible]
        description: The maximum amount of points received for answering this questionncorrectly
      - in: query
        name: question[position]
        description: The order in which the question will be displayed in the quiz
          in relationnto other questions
      - in: query
        name: question[question_name]
        description: The name of the question
      - in: query
        name: question[question_text]
        description: The text of the question
      - in: query
        name: question[question_type]
        description: The type of question
      - in: query
        name: question[quiz_group_id]
        description: The id of the quiz group to assign the question to
      - in: query
        name: question[text_after_answers]
        description: no description
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
  /courses/{course_id}/quizzes/quiz_id/questions/{id}:
    delete:
      summary: Delete a quiz question
      description: Delete a quiz question.
      operationId: delete-a-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-delete
      parameters:
      - in: query
        name: id
        description: The quiz question&#39;s unique identifier
      - in: query
        name: quiz_id
        description: The associated quiz&#39;s unique identifier
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
      - Id
    get:
      summary: Get a single quiz question
      description: Get a single quiz question.
      operationId: get-a-single-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-get
      parameters:
      - in: query
        name: id
        description: The quiz question unique identifier
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
      - Id
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