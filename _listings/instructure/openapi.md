---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Quiz Submissions API
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
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
  /quiz_submissions/{quiz_submission_id}/questions:
    get:
      summary: Get all quiz submission questions.
      description: Get all quiz submission questions..
      operationId: get-all-quiz-submission-questions
      x-api-path-slug: quiz-submissionsquiz-submission-idquestions-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the quiz submission question
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
    post:
      summary: Answering questions
      description: Answering questions.
      operationId: answering-questions
      x-api-path-slug: quiz-submissionsquiz-submission-idquestions-post
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: quiz_questions[]
        description: Set of question IDs and the answer value
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
  /quiz_submissions/{quiz_submission_id}/questions/id/flag:
    put:
      summary: Flagging a question.
      description: Flagging a question..
      operationId: flagging-a-question
      x-api-path-slug: quiz-submissionsquiz-submission-idquestionsidflag-put
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
      - Id
      - Flag
  /quiz_submissions/{quiz_submission_id}/questions/id/unflag:
    put:
      summary: Unflagging a question.
      description: Unflagging a question..
      operationId: unflagging-a-question
      x-api-path-slug: quiz-submissionsquiz-submission-idquestionsidunflag-put
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
      - Id
      - Unflag
---