---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Releases Search Security Headlines
  description: Search headlines for a company across all companies based on date,
    source, and title.
  version: v1
host: http://www.xignite.com/
basePath: xReleases.xml/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /SearchEvents:
    get:
      summary: Search Events
      description: Perform a complex query on events.
      operationId: postSearchevents
      x-api-path-slug: searchevents-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Events
  /SearchFutures:
    get:
      summary: Search Futures
      description: Returns futures match the name
      operationId: SearchFutures
      x-api-path-slug: searchfutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Futures
  /SearchIndicesByName:
    get:
      summary: Search Indices By Name
      description: Search indices by name.
      operationId: SearchIndicesByName
      x-api-path-slug: searchindicesbyname-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Indices
      - Name
  /SearchRates:
    get:
      summary: Search Rates
      description: Search rate names and description
      operationId: postSearchrates
      x-api-path-slug: searchrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Rates
  /SearchIPOBySymbol:
    get:
      summary: Search IPO By Symbol
      description: Post searchipobysymbol
      operationId: SearchIPOBySymbol
      x-api-path-slug: searchipobysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - IPO
      - Symbol
  /SearchIPOByName:
    get:
      summary: Search IPO By Name
      description: Post searchipobyname
      operationId: SearchIPOByName
      x-api-path-slug: searchipobyname-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - IPO
      - Name
  SearchMarketHeadlines/:
    get:
      summary: Search Market Headlines
      description: Search market headlines across all companies based on date, source,
        and title.
      operationId: getSearchmarketheadlines
      x-api-path-slug: searchmarketheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: Title
        description: Title of the headlines
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Market
      - Headlines
  SearchSecurityHeadlines/:
    get:
      summary: Search Security Headlines
      description: Search headlines for a company across all companies based on date,
        source, and title.
      operationId: getSearchsecurityheadlines
      x-api-path-slug: searchsecurityheadlines-get
      parameters:
      - in: query
        name: EndDate
        description: The end date range
      - in: query
        name: Identifier
        description: The ticker symbol for company
      - in: query
        name: IdentifierType
        description: The identifier to use
      - in: query
        name: Source
        description: The source of the news
      - in: query
        name: StartDate
        description: The start date range
      - in: query
        name: Title
        description: The title of the article
      - in: query
        name: _Token
        description: The API Key
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - Security
      - Headlines
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