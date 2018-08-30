---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Create a call broadcast
  description: Creates a call broadcast campaign using the Call Broadcast API. Send
    a CallBroadcast in the message body to add details in a voice broadcast campaign.
    The campaign can be created without contacts and bare minimum configuration, but
    contacts will have to be added further on to use the campaign
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
    post:
      summary: Send calls
      description: Use the /calls API to send individual calls quickly. A verified
        Caller ID and sufficient credits are required to make a call. CallRecipient
        represents a single recipient identified by phone number or contact id in
        CallFire system. You can attach user-defined attributes to a Call action via
        CallRecipient.attributes property, attributes are available in Call action
        response
      operationId: sendCalls
      x-api-path-slug: calls-post
      parameters:
      - in: body
        name: body
        description: An array of CallRecipient objects
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: campaignId
        description: Specifies a campaignId to send calls quickly on a previously
          created campaign
      - in: query
        name: defaultLiveMessage
        description: Text to be turned into a sound, this text will be played when
          the phone is answered
      - in: query
        name: defaultLiveMessageSoundId
        description: Id of sound file to play if phone is answered
      - in: query
        name: defaultMachineMessage
        description: Text to be turned into a sound, this text will be played when
          answering machine is detected
      - in: query
        name: defaultMachineMessageSoundId
        description: An id of a sound file to play if answering machine is detected
      - in: query
        name: defaultVoice
        description: The voice set by default for all text-to-speech messages defined
          in CallRecipient objects or as default *Message properties
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
  /calls/broadcasts:
    get:
      summary: Find call broadcasts
      description: Searches for all voice broadcasts created by user. Can query on
        label, name, and the current running status of the campaign. Returns a paged
        list of voice broadcasts
      operationId: findCallBroadcasts
      x-api-path-slug: callsbroadcasts-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: label
        description: A label of a voice broadcast
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name of voice broadcast
      - in: query
        name: offset
        description: Offset to the start of a given page
      - in: query
        name: running
        description: Specify whether the campaigns should be running or not
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
    post:
      summary: Create a call broadcast
      description: Creates a call broadcast campaign using the Call Broadcast API.
        Send a CallBroadcast in the message body to add details in a voice broadcast
        campaign. The campaign can be created without contacts and bare minimum configuration,
        but contacts will have to be added further on to use the campaign
      operationId: createCallBroadcast
      x-api-path-slug: callsbroadcasts-post
      parameters:
      - in: body
        name: body
        description: A CallBroadcast object
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: start
        description: Specify whether to immediately start this campaign (not required)
      - in: query
        name: strictValidation
        description: Turns on strict validation for recipients
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
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