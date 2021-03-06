swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
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
    put:
      summary: Update an existing quiz question
      description: Update an existing quiz question.
      operationId: update-an-existing-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-put
      parameters:
      - in: query
        name: id
        description: The quiz question&#39;s unique identifier
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