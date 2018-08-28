---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Get Question Answers
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
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/questions:
    get:
      summary: My Questions
      description: "Returns the questions owned by the user associated with the given
        access_token.\n \nThis method returns a list of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-this-method-returns-a
      x-api-path-slug: mequestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/featured:
    get:
      summary: My Questions Featured
      description: "Returns the questions that have active bounties offered by the
        user associated with the given access_token.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-that-have-active-bounties-offered-by-the-user-associated-with-the-given-access
      x-api-path-slug: mequestionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/no-answers:
    get:
      summary: My Questions No Answers
      description: "Returns the questions owned by the user associated with the given
        access_token that have no answers.\n \nThis method returns a list of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-have-no-answers-
      x-api-path-slug: mequestionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/unaccepted:
    get:
      summary: My Questions Unaccepted
      description: "Returns the questions owned by the user associated with the given
        access_token that have no accepted answer.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-have-no-accepted
      x-api-path-slug: mequestionsunaccepted-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/questions/unanswered:
    get:
      summary: My Questions Unanswered
      description: "Returns the questions owned by the user associated with the given
        access_token that are not considered answered.\n \nThis method returns a list
        of questions."
      operationId: returns-the-questions-owned-by-the-user-associated-with-the-given-access-token-that-are-not-consider
      x-api-path-slug: mequestionsunanswered-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /me/tags/{tags}/top-questions:
    get:
      summary: My Tags Top Questions
      description: "Returns the top 30 questions the user associated with the given
        access_token has posted in response to questions with the given tags.\n \nThis
        method returns a list of questions."
      operationId: returns-the-top-30-questions-the-user-associated-with-the-given-access-token-has-posted-in-response-
      x-api-path-slug: metagstagstopquestions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: path
        name: tags
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /me/top-question-tags:
    get:
      summary: My Top Question Tags
      description: "Returns the user identified by access_token's top 30 tags by question
        score.\n \nThis method returns a list of top tag objects."
      operationId: returns-the-user-identified-by-access-tokens-top-30-tags-by-question-score-this-method-returns-a-lis
      x-api-path-slug: metopquestiontags-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Tags
      - Questions
  /questions:
    get:
      summary: Get Questions
      description: "Gets all the questions on the site.\n \nThis method allows you
        make fairly flexible queries across the entire corpus of questions on a site.
        For example, getting all questions asked in the the week of Jan 1st 2011 with
        scores of 10 or more is a single query with parameters sort=votes&min=10&fromdate=1293840000&todate=1294444800.\n
        \nTo constrain questions returned to those with a set of tags, use the tagged
        parameter with a semi-colon delimited list of tags. This is an and contraint,
        passing tagged=c;java will return only those questions with both tags. As
        such, passing more than 5 tags will always return zero results.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        - hot - by the formula ordering the hot tab Does not accept min or max\n -
        week - by the formula ordering the week tab Does not accept min or max\n -
        month - by the formula ordering the month tab Does not accept min or max\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of questions."
      operationId: gets-all-the-questions-on-the-site-this-method-allows-you-make-fairly-flexible-queries-across-the-en
      x-api-path-slug: questions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          numbersort = hot => nonesort = week => nonesort = month => nonesort = relevance
          => none
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/featured:
    get:
      summary: Get Questions Featured
      description: "Returns all the questions with active bounties in the system.\n
        \nThe sorts accepted by this method operate on the follow fields of the question
        object:\n - activity - last_activity_date\n - creation - creation_date\n -
        votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: returns-all-the-questions-with-active-bounties-in-the-system-the-sorts-accepted-by-this-method-opera
      x-api-path-slug: questionsfeatured-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/no-answers:
    get:
      summary: Get Questions No Answers
      description: "Returns questions which have received no answers.\n \nCompare
        with /questions/unanswered which mearly returns questions that the sites consider
        insufficiently well answered.\n \nThis method corresponds roughly with the
        this site tab.\n \nTo constrain questions returned to those with a set of
        tags, use the tagged parameter with a semi-colon delimited list of tags. This
        is an and contraint, passing tagged=c;java will return only those questions
        with both tags. As such, passing more than 5 tags will always return zero
        results.\n \nThe sorts accepted by this method operate on the follow fields
        of the question object:\n - activity - last_activity_date\n - creation - creation_date\n
        - votes - score\n  activity is the default sort.\n \n It is possible to create
        moderately complex queries using sort, min, max, fromdate, and todate.\n \nThis
        method returns a list of questions."
      operationId: returns-questions-which-have-received-no-answers-compare-with-questionsunanswered-which-mearly-retur
      x-api-path-slug: questionsnoanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/unanswered:
    get:
      summary: Get Questions Unanswered
      description: "Returns questions the site considers to be unanswered.\n \nNote
        that just because a question has an answer, that does not mean it is considered
        answered. While the rules are subject to change, at this time a question must
        have at least one upvoted answer to be considered answered.\n \nTo constrain
        questions returned to those with a set of tags, use the tagged parameter with
        a semi-colon delimited list of tags. This is an and contraint, passing tagged=c;java
        will return only those questions with both tags. As such, passing more than
        5 tags will always return zero results.\n \nCompare with /questions/no-answers.\n
        \nThis method corresponds roughly with the unanswered tab.\n \nThe sorts accepted
        by this method operate on the follow fields of the question object:\n - activity
        - last_activity_date\n - creation - creation_date\n - votes - score\n  activity
        is the default sort.\n \n It is possible to create moderately complex queries
        using sort, min, max, fromdate, and todate.\n \nThis method returns a list
        of questions."
      operationId: returns-questions-the-site-considers-to-be-unanswered-note-that-just-because-a-question-has-an-answe
      x-api-path-slug: questionsunanswered-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: tagged
        description: String list (semicolon delimited)
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/{ids}:
    get:
      summary: Get Questions
      description: "Returns the questions identified in {ids}.\n \nThis is most useful
        for fetching fresh data when maintaining a cache of question ids, or polling
        for changes.\n \n{ids} can contain up to 100 semicolon delimited ids, to find
        ids programatically look for question_id on question objects.\n \nThe sorts
        accepted by this method operate on the follow fields of the question object:\n
        - activity - last_activity_date\n - creation - creation_date\n - votes - score\n
        \ activity is the default sort.\n \n It is possible to create moderately complex
        queries using sort, min, max, fromdate, and todate.\n \nThis method returns
        a list of questions."
      operationId: returns-the-questions-identified-in-ids-this-is-most-useful-for-fetching-fresh-data-when-maintaining
      x-api-path-slug: questionsids-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
  /questions/{ids}/answers:
    get:
      summary: Get Question Answers
      description: "Gets the answers to a set of questions identified in id.\n \nThis
        method is most useful if you have a set of interesting questions, and you
        wish to obtain all of their answers at once or if you are polling for new
        or updates answers (in conjunction with sort=activity).\n \n{ids} can contain
        up to 100 semicolon delimited ids, to find ids programatically look for question_id
        on question objects.\n \nThe sorts accepted by this method operate on the
        follow fields of the answer object:\n - activity - last_activity_date\n -
        creation - creation_date\n - votes - score\n  activity is the default sort.\n
        \n It is possible to create moderately complex queries using sort, min, max,
        fromdate, and todate.\n \nThis method returns a list of answers."
      operationId: gets-the-answers-to-a-set-of-questions-identified-in-id-this-method-is-most-useful-if-you-have-a-set
      x-api-path-slug: questionsidsanswers-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: fromdate
        description: Unix date
      - in: path
        name: ids
        description: Number list (semicolon delimited)
      - in: query
        name: max
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: min
        description: sort = activity => datesort = creation => datesort = votes =>
          number
      - in: query
        name: order
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      - in: query
        name: sort
      - in: query
        name: todate
        description: Unix date
      responses:
        200:
          description: OK
      tags:
      - Questions
      - Answers
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