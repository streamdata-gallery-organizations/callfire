---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find calls
  description: To search for all calls sent or received by the user. Use "id=0" for
    the campaignId parameter to query for all calls sent through the POST /calls API.
    See [call states and results](https://developers.callfire.com/results-responses-errors.html)
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls:
    get:
      summary: Find calls
      description: To search for all calls sent or received by the user. Use "id=0"
        for the campaignId parameter to query for all calls sent through the POST
        /calls API. See [call states and results](https://developers.callfire.com/results-responses-errors.html)
      operationId: findCalls
      x-api-path-slug: calls-get
      parameters:
      - in: query
        name: batchId
        description: An id of a contact batch, queries for calls of a particular contact
          batch
      - in: query
        name: campaignId
        description: An id of a campaign, queries for calls included to a particular
          campaign
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: fromNumber
        description: Phone number in E
      - in: query
        name: id
        description: Lists the Call ids to search for
      - in: query
        name: inbound
        description: Filters inbound calls for true value and outbound calls for false
          value
      - in: query
        name: intervalBegin
        description: Start of the find time interval, formatted in unix time milliseconds
      - in: query
        name: intervalEnd
        description: End of the find time interval, formatted in unix time milliseconds
      - in: query
        name: label
        description: A label for a specific call
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: results
        description: Searches for all calls with statuses listed in a comma separated
          string
      - in: query
        name: states
        description: Searches for all calls which correspond to statuses listed in
          a comma separated string
      - in: query
        name: toNumber
        description: Phone number in E
      responses:
        200:
          description: OK
      tags:
      - Calls
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