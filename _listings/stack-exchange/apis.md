---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You don???t have to read through a lot of discussion to find the best
  answer.    Like to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Questions
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange My Questions
  x-api-slug: stack-exchange
  description: "Returns the questions owned by the user associated with the given
    access_token.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/questions
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestions-get-openapi.md
- name: Stack Exchange My Questions Featured
  x-api-slug: stack-exchange
  description: "Returns the questions that have active bounties offered by the user
    associated with the given access_token.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/questions/featured
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsfeatured-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsfeatured-get-openapi.md
- name: Stack Exchange My Questions No Answers
  x-api-slug: stack-exchange
  description: "Returns the questions owned by the user associated with the given
    access_token that have no answers.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/questions/no-answers
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsnoanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsnoanswers-get-openapi.md
- name: Stack Exchange My Questions Unaccepted
  x-api-slug: stack-exchange
  description: "Returns the questions owned by the user associated with the given
    access_token that have no accepted answer.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/questions/unaccepted
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsunaccepted-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsunaccepted-get-openapi.md
- name: Stack Exchange My Questions Unanswered
  x-api-slug: stack-exchange
  description: "Returns the questions owned by the user associated with the given
    access_token that are not considered answered.\n \nThis method returns a list
    of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/questions/unanswered
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsunanswered-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/mequestionsunanswered-get-openapi.md
- name: Stack Exchange My Tags Top Questions
  x-api-slug: stack-exchange
  description: "Returns the top 30 questions the user associated with the given access_token
    has posted in response to questions with the given tags.\n \nThis method returns
    a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/tags/{tags}/top-questions
  tags: Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/metagstagstopquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/metagstagstopquestions-get-openapi.md
- name: Stack Exchange My Top Question Tags
  x-api-slug: stack-exchange
  description: "Returns the user identified by access_token's top 30 tags by question
    score.\n \nThis method returns a list of top tag objects."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//me/top-question-tags
  tags: Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/metopquestiontags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/metopquestiontags-get-openapi.md
- name: Stack Exchange Get Questions
  x-api-slug: stack-exchange
  description: "Gets all the questions on the site.\n \nThis method allows you make
    fairly flexible queries across the entire corpus of questions on a site. For example,
    getting all questions asked in the the week of Jan 1st 2011 with scores of 10
    or more is a single query with parameters sort=votes&min=10&fromdate=1293840000&todate=1294444800.\n
    \nTo constrain questions returned to those with a set of tags, use the tagged
    parameter with a semi-colon delimited list of tags. This is an and contraint,
    passing tagged=c;java will return only those questions with both tags. As such,
    passing more than 5 tags will always return zero results.\n \nThe sorts accepted
    by this method operate on the follow fields of the question object:\n - activity
    - last_activity_date\n - creation - creation_date\n - votes - score\n - hot -
    by the formula ordering the hot tab Does not accept min or max\n - week - by the
    formula ordering the week tab Does not accept min or max\n - month - by the formula
    ordering the month tab Does not accept min or max\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questions-get-openapi.md
- name: Stack Exchange Get Questions Featured
  x-api-slug: stack-exchange
  description: "Returns all the questions with active bounties in the system.\n \nThe
    sorts accepted by this method operate on the follow fields of the question object:\n
    - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
    \ activity is the default sort.\n \n It is possible to create moderately complex
    queries using sort, min, max, fromdate, and todate.\n \nThis method returns a
    list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/featured
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsfeatured-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsfeatured-get-openapi.md
- name: Stack Exchange Get Questions No Answers
  x-api-slug: stack-exchange
  description: "Returns questions which have received no answers.\n \nCompare with
    /questions/unanswered which mearly returns questions that the sites consider insufficiently
    well answered.\n \nThis method corresponds roughly with the this site tab.\n \nTo
    constrain questions returned to those with a set of tags, use the tagged parameter
    with a semi-colon delimited list of tags. This is an and contraint, passing tagged=c;java
    will return only those questions with both tags. As such, passing more than 5
    tags will always return zero results.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/no-answers
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsnoanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsnoanswers-get-openapi.md
- name: Stack Exchange Get Questions Unanswered
  x-api-slug: stack-exchange
  description: "Returns questions the site considers to be unanswered.\n \nNote that
    just because a question has an answer, that does not mean it is considered answered.
    While the rules are subject to change, at this time a question must have at least
    one upvoted answer to be considered answered.\n \nTo constrain questions returned
    to those with a set of tags, use the tagged parameter with a semi-colon delimited
    list of tags. This is an and contraint, passing tagged=c;java will return only
    those questions with both tags. As such, passing more than 5 tags will always
    return zero results.\n \nCompare with /questions/no-answers.\n \nThis method corresponds
    roughly with the unanswered tab.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/unanswered
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsunanswered-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsunanswered-get-openapi.md
- name: Stack Exchange Get Questions
  x-api-slug: stack-exchange
  description: "Returns the questions identified in {ids}.\n \nThis is most useful
    for fetching fresh data when maintaining a cache of question ids, or polling for
    changes.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
    programatically look for question_id on question objects.\n \nThe sorts accepted
    by this method operate on the follow fields of the question object:\n - activity
    - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
    is the default sort.\n \n It is possible to create moderately complex queries
    using sort, min, max, fromdate, and todate.\n \nThis method returns a list of
    questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}
  tags: Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsids-get-openapi.md
- name: Stack Exchange Get Question Answers
  x-api-slug: stack-exchange
  description: "Gets the answers to a set of questions identified in id.\n \nThis
    method is most useful if you have a set of interesting questions, and you wish
    to obtain all of their answers at once or if you are polling for new or updates
    answers (in conjunction with sort=activity).\n \n{ids} can contain up to 100 semicolon
    delimited ids, to find ids programatically look for question_id on question objects.\n
    \nThe sorts accepted by this method operate on the follow fields of the answer
    object:\n - activity - last_activity_date\n - creation - creation_date\n - votes
    - score\n  activity is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of answers."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}/answers
  tags: Questions,Answers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidsanswers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidsanswers-get-openapi.md
- name: Stack Exchange Get Question Comments
  x-api-slug: stack-exchange
  description: "Gets the comments on a question.\n \nIf you know that you have an
    question id and need the comments, use this method. If you know you have a answer
    id, use /answers/{ids}/comments. If you are unsure, use /posts/{ids}/comments.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for question_id on question objects.\n \nThe sorts accepted by this method
    operate on the follow fields of the comment object:\n - creation - creation_date\n
    - votes - score\n  creation is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of comments."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}/comments
  tags: Questions,Linked
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidscomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidscomments-get-openapi.md
- name: Stack Exchange Get Question Linked
  x-api-slug: stack-exchange
  description: "Gets questions which link to those questions identified in {ids}.\n
    \nThis method only considers questions that are linked within a site, and will
    never return questions from another Stack Exchange site.\n \nA question is considered
    \"linked\" when it explicitly includes a hyperlink to another question, there
    are no other heuristics.\n \n{ids} can contain up to 100 semicolon delimited ids,
    to find ids programatically look for question_id on question objects.\n \nThe
    sorts accepted by this method operate on the follow fields of the question object:\n
    - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
    - rank - a priority sort by site applies, subject to change at any time Does not
    accept min or max\n  activity is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}/linked
  tags: Questions,Linked
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidslinked-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidslinked-get-openapi.md
- name: Stack Exchange Get Question Related
  x-api-slug: stack-exchange
  description: "Returns questions that the site considers related to those identified
    in {ids}.\n \nThe algorithm for determining if questions are related is not documented,
    and subject to change at any time. Futhermore, these values are very heavily cached,
    and may not update immediately after a question has been editted. It is also not
    guaranteed that a question will be considered related to any number (even non-zero)
    of questions, and a consumer should be able to handle a variable number of returned
    questions.\n \n{ids} can contain up to 100 semicolon delimited ids, to find ids
    programatically look for question_id on question objects.\n \nThe sorts accepted
    by this method operate on the follow fields of the question object:\n - activity
    - last_activity_date\n - creation - creation_date\n - votes - score\n - rank -
    a priority sort by site applies, subject to change at any time Does not accept
    min or max\n  activity is the default sort.\n \n It is possible to create moderately
    complex queries using sort, min, max, fromdate, and todate.\n \nThis method returns
    a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}/related
  tags: Questions,Related
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidsrelated-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidsrelated-get-openapi.md
- name: Stack Exchange Get Question AnsweTimeliners
  x-api-slug: stack-exchange
  description: "Returns a subset of the events that have happened to the questions
    identified in id.\n \nThis provides data similar to that found on a question's
    timeline page.\n \nVoting data is scrubbed to deter inferencing of voter identity.\n
    \n{ids} can contain up to 100 semicolon delimited ids, to find ids programatically
    look for question_id on question objects.\n \nThis method returns a list of question
    timeline events."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//questions/{ids}/timeline
  tags: Questions,Timeline
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidstimeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/questionsidstimeline-get-openapi.md
- name: Stack Exchange Get User Questions
  x-api-slug: stack-exchange
  description: "Gets the questions asked by the users in {ids}.\n \n{ids} can contain
    up to 100 semicolon delimited ids, to find ids programatically look for user_id
    on user or shallow_user objects.\n \nThe sorts accepted by this method operate
    on the follow fields of the question object:\n - activity - last_activity_date\n
    - creation - creation_date\n - votes - score\n  activity is the default sort.\n
    \n It is possible to create moderately complex queries using sort, min, max, fromdate,
    and todate.\n \nThis method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{ids}/questions
  tags: Users,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/usersidsquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/usersidsquestions-get-openapi.md
- name: Stack Exchange Get User Tags Top Questions
  x-api-slug: stack-exchange
  description: "Returns the top 30 questions a user has asked with the given tags.\n
    \n{id} can contain a single id, to find it programatically look for user_id on
    user or shallow_user objects. {tags} is limited to 5 tags, passing more will result
    in an error.\n \nThe sorts accepted by this method operate on the follow fields
    of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
    - votes - score\n  activity is the default sort.\n \n It is possible to create
    moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
    method returns a list of questions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//users/{id}/tags/{tags}/top-questions
  tags: Users,Tags,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/usersidtagstagstopquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/usersidtagstagstopquestions-get-openapi.md
- name: Stack Exchange
  x-api-slug: stack-exchange
  description: After someone asks a question, members of the community propose answers.
    Others vote on those answers. Very quickly, the answers with the most votes rise
    to the top. You don???t have to read through a lot of discussion to find the best
    answer.    Like to...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Questions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/questions/master/_listings/stack-exchange/openapi.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---