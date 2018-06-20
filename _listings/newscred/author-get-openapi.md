---
swagger: "2.0"
x-collection-name: NewsCred
x-complete: 0
info:
  title: News Cred Author
  description: Returns an author that has written content available via this API.
  version: v1
host: api.newscred.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /topic/{guid]/articles/:
    get:
      summary: Topic Articles
      description: Returns a list of articles related to the specified topic.
      operationId: getTopicGu]Articles
      x-api-path-slug: topicguidarticles-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: article_filter_mode
        description: Enables article_filter_name and indicates filtering type
      - in: query
        name: article_filter_name
        description: Limit items to a predefined list of articles
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: from_date
        description: Beginning of date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: path
        name: guid
        description: The topic guid
      - in: query
        name: has_images
        description: Return only articles that have associated images (accessible
          via article/GUID/images)
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: pagesize
        description: Number of items to return
      - in: query
        name: sort
        description: Sort order for returned items
      - in: query
        name: sources
        description: List of sources to retrieve items from
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: query
        name: to_date
        description: End of date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Topic
      - Articles
  articles/:
    get:
      summary: Articles
      description: Returns a list of articles according to the specified set of parameters.
      operationId: getArticles
      x-api-path-slug: articles-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: article_filter_mode
        description: Enables article_filter_name and indicates filtering type
      - in: query
        name: article_filter_name
        description: Limit items to a predefined list of articles
      - in: query
        name: boolean_operator
        description: Indicates the boolean operation to use on search keywords that
          do not have explicit whitelist (+) or blacklist (-) operators on them
      - in: query
        name: categories
        description: Limit items to the categories specified
      - in: query
        name: exact
        description: If this parameter is not specified, then stemming is applied,
          so that for example the query term ship matches articles containing shipping,
          and vice versa
      - in: query
        name: from_date
        description: Beginning of publication date range for which items are searched
      - in: query
        name: get_topics
        description: Set to true to include associated topics inline with each article
      - in: query
        name: has_images
        description: Sort order for returned items
      - in: query
        name: languages
        description: Limit items to those in the specified language
      - in: query
        name: licensed
        description: Search exclusively for fully licensed, full text content
      - in: query
        name: links
        description: Value is a space delimited list of article links
      - in: query
        name: max_length
        description: Returns only articles with at most this many words
      - in: query
        name: media_types
        description: Limit the media type of the returned items
      - in: query
        name: min_length
        description: Returns only articles with at least this many words
      - in: query
        name: mm
        description: 'Minimum Match: specifies how many of the non whitelist/blacklist
          keywords must match for an article to be included in the results'
      - in: query
        name: modified_since
        description: Get only articles that have been modified since the supplied
          date
      - in: query
        name: offset
        description: Number of items to skip before beginning the result set
      - in: query
        name: query
        description: Specifies the set of words and phrases to search for
      - in: query
        name: query_fields
        description: Specifies which field to search when searching for articles
      - in: query
        name: safe_search
        description: Removes articles containing offensive words from search result;
          when set to true
      - in: query
        name: sort
        description: Sort order for returned items
      - in: query
        name: sources
        description: Limit items to the sources specified
      - in: query
        name: source_countries
        description: Search against only sources from the specified countries
      - in: query
        name: source_filter_mode
        description: Enables source_filter_name and indicates filtering type
      - in: query
        name: source_filter_name
        description: Limit items to a predefined list of sources
      - in: query
        name: topics
        description: Value is a space delimited list of topic guids
      - in: query
        name: topic_filter_mode
        description: Enables topic_filter_name and indicates filtering type
      - in: query
        name: topic_filter_name
        description: Limit items to a predefined list of topics
      - in: query
        name: to_date
        description: End of publication date range for which items are searched
      responses:
        200:
          description: OK
      tags:
      - News
      - Articles
  author/:
    get:
      summary: Author
      description: Returns an author that has written content available via this API.
      operationId: getAuthor
      x-api-path-slug: author-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      responses:
        200:
          description: OK
      tags:
      - Author
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