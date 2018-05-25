---
name: CallFire
x-slug: callfire
description: Grow your business with virtual phone numbers, IVR, voice broadcasting,
  mass text messaging services and power dialing. Try CallFire for FREE!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
x-kinRank: "9"
x-alexaRank: "129466"
tags: CallFire
created: "2018-05-25"
modified: "2018-05-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/apis.md
specificationVersion: "0.14"
apis:
- name: Callfire Find calls
  x-api-slug: callfire
  description: To search for all calls sent or received by the user. Use "id=0" for
    the campaignId parameter to query for all calls sent through the POST /calls API.
    See [call states and results](https://developers.callfire.com/results-responses-errors.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls
  tags: Calls
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/calls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/calls-get-openapi.md
- name: Callfire Send calls
  x-api-slug: callfire
  description: Use the /calls API to send individual calls quickly. A verified Caller
    ID and sufficient credits are required to make a call. CallRecipient represents
    a single recipient identified by phone number or contact id in CallFire system.
    You can attach user-defined attributes to a Call action via CallRecipient.attributes
    property, attributes are available in Call action response
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls
  tags: Calls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/calls-post-openapi.md
- name: Callfire Find call broadcasts
  x-api-slug: callfire
  description: Searches for all voice broadcasts created by user. Can query on label,
    name, and the current running status of the campaign. Returns a paged list of
    voice broadcasts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts
  tags: Calls,Broadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcasts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcasts-get-openapi.md
- name: Callfire Create a call broadcast
  x-api-slug: callfire
  description: Creates a call broadcast campaign using the Call Broadcast API. Send
    a CallBroadcast in the message body to add details in a voice broadcast campaign.
    The campaign can be created without contacts and bare minimum configuration, but
    contacts will have to be added further on to use the campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts
  tags: Calls,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcasts-post-openapi.md
- name: Callfire Find a specific call broadcast
  x-api-slug: callfire
  description: Returns a single CallBroadcast instance for a given call broadcast
    campaign id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}
  tags: Calls,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsid-get-openapi.md
- name: Callfire Update a call broadcast
  x-api-slug: callfire
  description: This operation lets the user modify the configuration of a voice broadcast
    campaign after call broadcast campaign is created. See CallBroadcast for more
    information on what can/can't be updated on this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}
  tags: Calls,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsid-put-openapi.md
- name: Callfire Archive voice broadcast
  x-api-slug: callfire
  description: Archives a voice broadcast (voice broadcast will be hidden in search
    results)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/archive
  tags: Calls,Broadcasts,Archive
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidarchive-post-openapi.md
- name: Callfire Find batches in a call broadcast
  x-api-slug: callfire
  description: This endpoint will enable the user to page through all of the batches
    for a particular voice broadcast campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/batches
  tags: Calls,Broadcasts,Batches
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidbatches-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidbatches-get-openapi.md
- name: Callfire Add batches to a call broadcast
  x-api-slug: callfire
  description: The 'add batch' API allows user to add additional batches to an already
    created voice broadcast campaign. The added batch will go through the CallFire
    validation process, unlike in the recipients version of this API. That is why
    you can use the scrubDuplicates flag to remove duplicates from your batch. Batches
    may be added as a contact list id, a list of contact ids, or a list of numbers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/batches
  tags: Calls,Broadcasts,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidbatches-post-openapi.md
- name: Callfire Find calls in a call broadcast
  x-api-slug: callfire
  description: This endpoint will enable the user to page through all calls for a
    particular call broadcast campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/calls
  tags: Calls,Broadcasts,Calls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidcalls-get-openapi.md
- name: Callfire Add recipients to a call broadcast
  x-api-slug: callfire
  description: Use this API to add the recipients to an existing voice broadcast.
    Post a list of Recipient objects to be added to the voice broadcast campaign.
    These contacts will not go through validation process, and will be acted upon
    as they are added. Recipients may be added as a list of contact ids, or list of
    numbers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/recipients
  tags: Calls,Broadcasts,Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidrecipients-post-openapi.md
- name: Callfire Start voice broadcast
  x-api-slug: callfire
  description: Start a voice broadcast
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/start
  tags: Calls,Broadcasts,Start
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidstart-post-openapi.md
- name: Callfire Get statistics on call broadcast
  x-api-slug: callfire
  description: Returns broadcast statistics like total number of sent/received actions,
    total cost, number of remaining outbound actions, error count, etc
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/stats
  tags: Calls,Broadcasts,Stats
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidstats-get-openapi.md
- name: Callfire Stop voice broadcast
  x-api-slug: callfire
  description: Stop a voice broadcast
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/broadcasts/{id}/stop
  tags: Calls,Broadcasts,Stop
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsbroadcastsidstop-post-openapi.md
- name: Callfire Get call recording by id
  x-api-slug: callfire
  description: Returns metadata of recording of a particular call. Metadata contains
    a link to a MP3 recording
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/recordings/{id}
  tags: Calls,Recordings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsrecordingsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsrecordingsid-get-openapi.md
- name: Callfire Get call recording in mp3 format
  x-api-slug: callfire
  description: Returns an MP3 recording of particular call, response contains binary
    data, content type is 'audio/mpeg'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/recordings/{id}.mp3
  tags: Calls,Recordings.mp3
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsrecordingsid-mp3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsrecordingsid-mp3-get-openapi.md
- name: Callfire Find a specific call
  x-api-slug: callfire
  description: Returns a single Call instance for a given call id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/{id}
  tags: Calls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsid-get-openapi.md
- name: Callfire Get call recordings for a call
  x-api-slug: callfire
  description: Returns a list of recordings metadata of particular call. Metadata
    contains link to a MP3 recording
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/{id}/recordings
  tags: Calls,Recordings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordings-get-openapi.md
- name: Callfire Get call recording by name
  x-api-slug: callfire
  description: Returns recording metadata of particular call. Metadata contains link
    to a MP3 recording
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/{id}/recordings/{name}
  tags: Calls,Recordings,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordingsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordingsname-get-openapi.md
- name: Callfire Get call mp3 recording by name
  x-api-slug: callfire
  description: Returns a MP3 recording of a particular call, response contains binary
    data, content type is 'audio/mpeg'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//calls/{id}/recordings/{name}.mp3
  tags: Calls,Recordings,Name.mp3
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordingsname-mp3-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/callsidrecordingsname-mp3-get-openapi.md
- name: Callfire Find a specific batch
  x-api-slug: callfire
  description: Returns a single Batch instance for a given batch id. This API is useful
    for determining the state of a validating batch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/batches/{id}
  tags: Campaigns,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignsbatchesid-get-openapi.md
- name: Callfire Update a batch
  x-api-slug: callfire
  description: Updates a single Batch instance, currently batch can only be turned
    "on/off"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/batches/{id}
  tags: Campaigns,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignsbatchesid-put-openapi.md
- name: Callfire Find sounds
  x-api-slug: callfire
  description: To find all campaign sounds which were created by user. Returns all
    sounds available to be used in campaigns
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssounds-get-openapi.md
- name: Callfire Add sound via call
  x-api-slug: callfire
  description: Use this API to create a sound via a phone call. Provide the required
    phone number in the CallCreateSound object inside the request, and user will receive
    a call shortly after with instructions on how to record a sound over the phone.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/calls
  tags: Campaigns,Sounds,Calls
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundscalls-post-openapi.md
- name: Callfire Add sound via file
  x-api-slug: callfire
  description: Create a campaign sound file via a supplied .mp3 or .wav file
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/files
  tags: Campaigns,Sounds,Files
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundsfiles-post-openapi.md
- name: Callfire Add sound via text-to-speech
  x-api-slug: callfire
  description: 'Use this API to create a sound file via a supplied string of text.
    Add a text in the TextToSpeech.message field, and pick a voice in the TextToSpeech.voice
    field. Available voices are: MALE1, FEMALE1, FEMALE2, SPANISH1, FRENCHCANADIAN1'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/tts
  tags: Campaigns,Sounds,Tts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundstts-post-openapi.md
- name: Callfire Delete a specific sound
  x-api-slug: callfire
  description: Deletes a single campaign sound instance for a specific campaign sound
    id, this operation does not delete sound completely, it sets sound status to ARCHIVED
    which means that sound will no longer appear in 'find' operation results, but
    still accessible via 'get' operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundsid-delete-openapi.md
- name: Callfire Find a specific sound
  x-api-slug: callfire
  description: Returns a single CampaignSound instance for a given sound id in campaign.
    This is a meta data to the sounds. No audio data is returned from this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}
  tags: Campaigns,Sounds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundsid-get-openapi.md
- name: Callfire Download a MP3 sound
  x-api-slug: callfire
  description: Download the MP3 version of a hosted file. This is an audio data endpoint.
    Returns binary response of the 'audio/mpeg' content type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}.mp3
  tags: Campaigns,Sounds.mp3
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundsid-mp3-get-openapi.md
- name: Callfire Download a WAV sound
  x-api-slug: callfire
  description: Download the WAV version of the hosted file. This is an audio data
    endpoint. Returns binary response of the 'audio/mpeg' content type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//campaigns/sounds/{id}.wav
  tags: Campaigns,Sounds.wav
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/campaignssoundsid-wav-get-openapi.md
- name: Callfire Find contacts
  x-api-slug: callfire
  description: Find user's contacts by id, contact list, or on any property name.
    Returns a paged list of contacts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts
  tags: Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contacts-get-openapi.md
- name: Callfire Create contacts
  x-api-slug: callfire
  description: Creates contacts in CallFire system. These contacts are not validated
    on creation. They will be validated upon being added to a campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts
  tags: Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contacts-post-openapi.md
- name: Callfire Find do not contact (dnc) items
  x-api-slug: callfire
  description: Searches for all Do Not Contact (DNC) objects created by user. These
    DoNotContact entries only affect calls/texts/campaigns on this account. Returns
    a paged list of DoNotContact objects
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs
  tags: Contacts,Dncs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncs-get-openapi.md
- name: Callfire Add or update do not contact (dnc) numbers
  x-api-slug: callfire
  description: Add or update a list of Do Not Contact (DNC) contact entries. Can toggle
    whether the DNCs are enabled for calls/texts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs
  tags: Contacts,Dncs
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncs-post-openapi.md
- name: Callfire Delete do not contact (dnc) numbers contained in source.
  x-api-slug: callfire
  description: Delete Do Not Contact (DNC) contact entries contained in source.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs/sources/{source}
  tags: Contacts,Dncs,Sources,Source
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncssourcessource-delete-openapi.md
- name: Callfire Find universal do not contacts (udnc) associated with toNumber
  x-api-slug: callfire
  description: Searches for a UniversalDoNotContact object for a given phone number.
    Shows whether inbound/outbound actions are allowed for a given number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs/universals/{toNumber}
  tags: Contacts,Dncs,Universals,ToNumber
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncsuniversalstonumber-get-openapi.md
- name: Callfire Delete do not contact (dnc) number. If number contains commas treat
    as list of numbers
  x-api-slug: callfire
  description: Delete a Do Not Contact (DNC) contact entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs/{number}
  tags: Contacts,Dncs,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncsnumber-delete-openapi.md
- name: Callfire Get do not contact (dnc)
  x-api-slug: callfire
  description: Get Do Not Contact (DNC) object create by user. This DoNotContact entry
    only affects calls/texts/campaigns on this account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs/{number}
  tags: Contacts,Dncs,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncsnumber-get-openapi.md
- name: Callfire Update an individual do not contact (dnc) number
  x-api-slug: callfire
  description: Update a Do Not Contact (DNC) contact entry. Can toggle whether the
    DNC is enabled for calls/texts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/dncs/{number}
  tags: Contacts,Dncs,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsdncsnumber-put-openapi.md
- name: Callfire Find contact lists
  x-api-slug: callfire
  description: Searches for all contact lists which are available for the current
    user. Returns a paged list of contact lists
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslists-get-openapi.md
- name: Callfire Create contact lists
  x-api-slug: callfire
  description: Creates a contact list for use with campaigns using 1 of 3 inputs.
    A List of Contact objects, a list of String E.164 numbers, or a list of CallFire
    contactIds can be used as the data source for the created contact list. After
    contact list is added into the CallFire system, contact lists goes through seven
    system safeguards that check the accuracy and consistency of the data. For example,
    our system checks that contact number is formatted correctly, is valid, is not
    duplicated in another contact list, or is not added on a specific DNC list. You
    can configure to keep/merge or remove contacts which do not complies these rules.
    If contacts were not added to a contact list after the validation, this means
    the data needs to be properly formatted and corrected before calling this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslists-post-openapi.md
- name: Callfire Create contact list from file
  x-api-slug: callfire
  description: Creates a contact list to be used with campaigns through uploading
    a .csv file. Returns the id of created list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/upload
  tags: Contacts,Lists,Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsupload-post-openapi.md
- name: Callfire Delete a contact list
  x-api-slug: callfire
  description: Deletes a contact list, included contacts will not be deleted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsid-delete-openapi.md
- name: Callfire Find a specific contact list
  x-api-slug: callfire
  description: Returns a single ContactList instance for a given contact list id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsid-get-openapi.md
- name: Callfire Update a contact list
  x-api-slug: callfire
  description: Updates contact list instance.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsid-put-openapi.md
- name: Callfire Delete contacts from a contact list
  x-api-slug: callfire
  description: Deletes contacts from a contact list. List the contact ids in request
    to delete multiple contacts with one request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsiditems-delete-openapi.md
- name: Callfire Find contacts in a contact list
  x-api-slug: callfire
  description: Searches for all entries in a contact list with specified id. Returns
    a paged list of contact entries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsiditems-get-openapi.md
- name: Callfire Add contacts to a contact list
  x-api-slug: callfire
  description: 'Adds contacts to a contact list. Available contact sources are: list
    of the contact entities, list of ids of existing contacts in user''s account,
    list of phone numbers in E.164 format (11-digits)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsiditems-post-openapi.md
- name: Callfire Delete a contact from a contact list
  x-api-slug: callfire
  description: Deletes a single contact from a contact list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items/{contactId}
  tags: Contacts,Lists,Items,ContactId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactslistsiditemscontactid-delete-openapi.md
- name: Callfire Delete a contact
  x-api-slug: callfire
  description: Deletes a contact instance from account
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/{id}
  tags: Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsid-delete-openapi.md
- name: Callfire Find a specific contact
  x-api-slug: callfire
  description: Returns a Contact instance for a given contact id. Deleted contacts
    can be still retrieved but will be marked as deleted. Deleted contacts will not
    be shown in search request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/{id}
  tags: Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsid-get-openapi.md
- name: Callfire Update a contact
  x-api-slug: callfire
  description: Updates a single contact instance with id specified
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/{id}
  tags: Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsid-put-openapi.md
- name: Callfire Find a contact's history
  x-api-slug: callfire
  description: Searches for all texts and calls attributed to a contact. Returns a
    list of calls and texts a contact has been involved with
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/{id}/history
  tags: Contacts,History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/contactsidhistory-get-openapi.md
- name: Callfire Find keywords
  x-api-slug: callfire
  description: Searches for all keywords available for purchase on the CallFire platform.
    If a keyword appears in the response, it is available for purchase. List the 'keywords'
    in a query parameter to search for multiple keywords (at least one keyword should
    be sent in request)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords
  tags: Keywords
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywords-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywords-get-openapi.md
- name: Callfire Find keyword leases
  x-api-slug: callfire
  description: Searches for all keywords owned by user. A keyword lease is the ownership
    information involving a keyword
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases
  tags: Keywords,Leases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordsleases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordsleases-get-openapi.md
- name: Callfire Find a specific lease
  x-api-slug: callfire
  description: Searches for all keywords owned by user
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases/{keyword}
  tags: Keywords,Leases,Keyword
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordsleaseskeyword-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordsleaseskeyword-get-openapi.md
- name: Callfire Update a lease
  x-api-slug: callfire
  description: Updates a keyword lease. Turns the autoRenew on/off.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/leases/{keyword}
  tags: Keywords,Leases,Keyword
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordsleaseskeyword-put-openapi.md
- name: Callfire Check for a specific keyword
  x-api-slug: callfire
  description: Searches for the specific keyword to purchase on the CallFire platform.
    Returns 'true' if keyword is available.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//keywords/{keyword}/available
  tags: Keywords,Keyword,Available
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/keywordskeywordavailable-get-openapi.md
- name: Callfire Find account details
  x-api-slug: callfire
  description: Searches for the user account details. Details include name, email,
    and basic account permissions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/account
  tags: Me,Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/meaccount-get-openapi.md
- name: Callfire Find api credentials
  x-api-slug: callfire
  description: Searches for all credentials generated by user. Returns a paged list
    of the API credentials. Only ACCOUNT_HOLDER can invoke this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/api/credentials
  tags: Me,Api,Credentials
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/meapicredentials-get-openapi.md
- name: Callfire Create api credentials
  x-api-slug: callfire
  description: Creates an API credentials for the CallFire API. This endpoint requires
    full CallFire account credentials to be used, authenticated using Basic Authentication.
    At the moment user provides only the name for the credentials. The generated credentials
    can be used to access any CallFire APIs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/api/credentials
  tags: Me,Api,Credentials
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/meapicredentials-post-openapi.md
- name: Callfire Delete api credentials
  x-api-slug: callfire
  description: Deletes a specified API credential. Currently, removes the ability
    to access the API. Only ACCOUNT_HOLDER can invoke this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/api/credentials/{id}
  tags: Me,Api,Credentials
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/meapicredentialsid-delete-openapi.md
- name: Callfire Find a specific api credential
  x-api-slug: callfire
  description: Returns an API credential instance for a given api credential id. Only
    ACCOUNT_HOLDER can invoke this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/api/credentials/{id}
  tags: Me,Api,Credentials
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/meapicredentialsid-get-openapi.md
- name: Callfire Find credit usage
  x-api-slug: callfire
  description: Find credit usage for the user. Returns credits usage for time period
    specified or if unspecified then total for all time.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/billing/credit-usage
  tags: Me,Billing,Credit-usage
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mebillingcreditusage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mebillingcreditusage-get-openapi.md
- name: Callfire Find plan usage
  x-api-slug: callfire
  description: Searches for the data of a billing plan usage for the user. Returns
    the data of a billing plan usage for the current month
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/billing/plan-usage
  tags: Me,Billing,Plan-usage
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mebillingplanusage-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mebillingplanusage-get-openapi.md
- name: Callfire Find caller ids
  x-api-slug: callfire
  description: Returns a list of verified caller ids. If the number is not shown in
    the list, then it is not verified. In this case sending of a verification code
    is required.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/callerids
  tags: Me,Callerids
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mecallerids-get-openapi.md
- name: Callfire Create a caller id
  x-api-slug: callfire
  description: Generates and sends a verification code to the phone number provided
    in the path. The verification code is delivered via a phone call. This code needs
    to be submitted to the verify caller id API endpoint to complete verification.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/callerids/{callerid}
  tags: Me,Callerids,Callerid
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mecalleridscallerid-post-openapi.md
- name: Callfire Verify a caller id
  x-api-slug: callfire
  description: With the verification code received from the Create caller id endpoint,
    a call to this endpoint is required to finish verification
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//me/callerids/{callerid}/verification-code
  tags: Me,Callerids,Callerid,Verification-code
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mecalleridscalleridverificationcode-post-openapi.md
- name: Callfire Create media
  x-api-slug: callfire
  description: 'Uploads media file to account, acceptable media formats: bmp, gif,
    jpg, m4a, mp3, mp4, png, wav'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//media
  tags: Media
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/media-post-openapi.md
- name: Callfire Download media by extension
  x-api-slug: callfire
  description: 'Download a media file. Available types of files: bmp, gif, jpg, m4a,
    mp3, mp4, png, wav. Content type in response depends on ''extension'' parameter,
    e.g. image/jpeg, image/png, audio/mp3, etc'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//media/public/{key}.{extension}
  tags: Media,Public,Key.extension
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mediapublickey-extension-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mediapublickey-extension-get-openapi.md
- name: Callfire Get a specific media
  x-api-slug: callfire
  description: Get media resource by id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//media/{id}
  tags: Media
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mediaid-get-openapi.md
- name: Callfire Download media by extension
  x-api-slug: callfire
  description: 'Download a media file. Available types of files: bmp, gif, jpg, m4a,
    mp3, mp4, png, wav. Content type in response depends on ''extension'' parameter,
    e.g. image/jpeg, image/png, audio/mp3, etc'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//media/{id}.{extension}
  tags: Media,Extensions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mediaid-extension-get-openapi.md
- name: Callfire Download a MP3 media
  x-api-slug: callfire
  description: Download a MP3 media, endpoint returns application/binary content-type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//media/{id}/file
  tags: Media,File
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/mediaidfile-get-openapi.md
- name: Callfire Find leases
  x-api-slug: callfire
  description: Searches for all numbers leased by account user. This API is useful
    for finding all numbers currently owned by the user. Returns a paged list of number
    leases.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases
  tags: Numbers,Leases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleases-get-openapi.md
- name: Callfire Find lease configs
  x-api-slug: callfire
  description: Searches for all number lease configs for the user. Returns a paged
    list of NumberConfig
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases/configs
  tags: Numbers,Leases,Configs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesconfigs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesconfigs-get-openapi.md
- name: Callfire Find a specific lease config
  x-api-slug: callfire
  description: Returns a single NumberConfig instance for a given number lease
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases/configs/{number}
  tags: Numbers,Leases,Configs,Number
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesconfigsnumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesconfigsnumber-get-openapi.md
- name: Callfire Update a lease config
  x-api-slug: callfire
  description: Updates a phone number lease configuration. Use this API endpoint to
    add an Inbound IVR or Call Tracking feature to a CallFire phone number. Call tracking
    configuration allows you to track the incoming calls, to analyze and to respond
    customers using sms or voice replies. For more information see [call tracking
    page](https://www.callfire.com/products/call-tracking)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases/configs/{number}
  tags: Numbers,Leases,Configs,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesconfigsnumber-put-openapi.md
- name: Callfire Find a specific lease
  x-api-slug: callfire
  description: Returns a single NumberLease instance for a given number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases/{number}
  tags: Numbers,Leases,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesnumber-get-openapi.md
- name: Callfire Update a lease
  x-api-slug: callfire
  description: Updates a number lease instance. Ability to turn on/off autoRenew and
    toggle call/text features for a particular number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/leases/{number}
  tags: Numbers,Leases,Number
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersleasesnumber-put-openapi.md
- name: Callfire Find local numbers
  x-api-slug: callfire
  description: Searches for numbers available for purchase in CallFire local numbers
    catalog . At least one additional parameter is required. User may filter local
    numbers by their region information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/local
  tags: Numbers,Local
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numberslocal-get-openapi.md
- name: Callfire Find number regions
  x-api-slug: callfire
  description: Searches for region information. Use this API to obtain detailed region
    information that can be used to query for more specific phone numbers than a general
    query.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/regions
  tags: Numbers,Regions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numbersregions-get-openapi.md
- name: Callfire Find tollfree numbers
  x-api-slug: callfire
  description: Searches for the toll free numbers which are available for purchase
    in the CallFire catalog
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//numbers/tollfree
  tags: Numbers,Tollfree
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/numberstollfree-get-openapi.md
- name: Callfire Purchase keywords
  x-api-slug: callfire
  description: Purchase keywords. Send a list of available keywords into this API
    to purchase them using CallFire credits. Make sure the account has enough credits
    before trying to purchase the keywords
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//orders/keywords
  tags: Orders,Keywords
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/orderskeywords-post-openapi.md
- name: Callfire Purchase numbers
  x-api-slug: callfire
  description: Purchase numbers. There are many ways to purchase a number. Set either
    'tollFreeCount' or 'localCount' along with some querying fields to purchase numbers
    by bulk query. Set the list of numbers to purchase by list. Available numbers
    will be purchased using CallFire credits owned by the user. Make sure the account
    has enough credits before trying to purchase
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//orders/numbers
  tags: Orders,Numbers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/ordersnumbers-post-openapi.md
- name: Callfire Find a specific order
  x-api-slug: callfire
  description: Returns a single NumberOrder instance for a given order id. Order contains
    information about purchased keywords, local, toll-free numbers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//orders/{id}
  tags: Orders
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/ordersid-get-openapi.md
- name: Callfire Find texts
  x-api-slug: callfire
  description: Searches for texts sent or received by user. Use "campaignId=0" parameter
    to query for all texts sent through the POST /texts API. See [call states and
    results](https://developers.callfire.com/results-responses-errors.html)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts
  tags: Texts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/texts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/texts-get-openapi.md
- name: Callfire Send texts
  x-api-slug: callfire
  description: Use the /texts API to send individual texts quickly. By default all
    texts are going out from CallFire's dedicated short code 67076
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts
  tags: Texts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/texts-post-openapi.md
- name: Callfire Find auto replies
  x-api-slug: callfire
  description: Find all text autoreplies created by user. Returns a paged list of
    TextAutoReply
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/auto-replys
  tags: Texts,Auto-replys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsautoreplys-get-openapi.md
- name: Callfire Create an auto reply
  x-api-slug: callfire
  description: CallFire gives you possibility to set up auto reply messages for your
    numbers and keywords. You can set a general auto reply for anyone who texts your
    number, keyword, and/or include a text to match, so that the auto reply would
    be sent only to those who text the matched text
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/auto-replys
  tags: Texts,Auto-replys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsautoreplys-post-openapi.md
- name: Callfire Delete an auto reply
  x-api-slug: callfire
  description: Deletes a text auto reply and removes the configuration. Can not delete
    a TextAutoReply which is currently active for a campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/auto-replys/{id}
  tags: Texts,Auto-replys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsautoreplysid-delete-openapi.md
- name: Callfire Find a specific auto reply
  x-api-slug: callfire
  description: Returns a single TextAutoReply instance for a given text auto reply
    id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/auto-replys/{id}
  tags: Texts,Auto-replys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsautoreplysid-get-openapi.md
- name: Callfire Find text broadcasts
  x-api-slug: callfire
  description: Searches for all text broadcasts created by user. Can query on label,
    name, and the current running status of the campaign. Returns a paged list of
    text broadcasts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts
  tags: Texts,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcasts-get-openapi.md
- name: Callfire Create a text broadcast
  x-api-slug: callfire
  description: Creates a text broadcast campaign using the Text Broadcast API. Send
    a TextBroadcast object in the message body to detail a text broadcast campaign.
    A campaign can be created without contacts and with bare minimum configuration,
    but contacts have to be added further on to use the campaign. It supports scheduling,
    retry logic, pattern-based messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts
  tags: Texts,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcasts-post-openapi.md
- name: Callfire Find a specific text broadcast
  x-api-slug: callfire
  description: Returns a single TextBroadcast instance for a given text broadcast
    id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}
  tags: Texts,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsid-get-openapi.md
- name: Callfire Update a text broadcast
  x-api-slug: callfire
  description: Allows modifying the configuration of existing text broadcast campaign.
    See TextBroadcast for more information on what can/can't be updated on this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}
  tags: Texts,Broadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsid-put-openapi.md
- name: Callfire Archive text broadcast
  x-api-slug: callfire
  description: Archives a text broadcast (and hides it in the search results)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/archive
  tags: Texts,Broadcasts,Archive
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidarchive-post-openapi.md
- name: Callfire Find batches in a text broadcast
  x-api-slug: callfire
  description: This endpoint will enable the user to page through all of the batches
    for a particular text broadcast campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/batches
  tags: Texts,Broadcasts,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidbatches-get-openapi.md
- name: Callfire Add batches to a text broadcast
  x-api-slug: callfire
  description: Allows adding an extra batches to an already created text broadcast
    campaign. The batches which being  added pass the CallFire validation process
    (unlike in the recipients version of this API). That is why using of a scrubDuplicates
    flag remove duplicates from your batch. Batches may be added as a contact list
    id, a list of contact ids, or a list of numbers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/batches
  tags: Texts,Broadcasts,Batches
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidbatches-post-openapi.md
- name: Callfire Add recipients to a text broadcast
  x-api-slug: callfire
  description: Use this API to add recipients to a text broadcast which is already
    created. Post a list of Recipient objects to be immediately added to the text
    broadcast campaign. These contacts will not go through validation process, and
    will be acted upon as they are added. Recipients may be added as a list of contact
    ids, or list of numbers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/recipients
  tags: Texts,Broadcasts,Recipients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidrecipients-post-openapi.md
- name: Callfire Start text broadcast
  x-api-slug: callfire
  description: Starts a text broadcast
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/start
  tags: Texts,Broadcasts,Start
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidstart-post-openapi.md
- name: Callfire Get statistics on text broadcast
  x-api-slug: callfire
  description: 'Returns the broadcast statistics. Example: total number of the sent/received
    actions, total cost, number of remaining outbound actions, error count, etc'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/stats
  tags: Texts,Broadcasts,Stats
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidstats-get-openapi.md
- name: Callfire Stop text broadcast
  x-api-slug: callfire
  description: Stops a text broadcast
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/stop
  tags: Texts,Broadcasts,Stop
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidstop-post-openapi.md
- name: Callfire Find texts in a text broadcast
  x-api-slug: callfire
  description: This endpoint will enable the user to page through all of the texts
    for a particular text broadcast campaign
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/broadcasts/{id}/texts
  tags: Texts,Broadcasts,Texts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsbroadcastsidtexts-get-openapi.md
- name: Callfire Find a specific text
  x-api-slug: callfire
  description: Returns a single Text instance for a given text id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//texts/{id}
  tags: Texts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/textsid-get-openapi.md
- name: Callfire Find webhooks
  x-api-slug: callfire
  description: Searches all webhooks available for a current user. Searches by name,
    resource, event, callback URL, or whether they are enabled. Returns a paged list
    of Webhooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks
  tags: Webhooks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooks-get-openapi.md
- name: Callfire Create a webhook
  x-api-slug: callfire
  description: 'Create a Webhook for notification in the CallFire system. Use the
    webhooks API to receive notifications of important CallFire events. Select the
    resource to listen to, and then choose the resource events to receive notifications
    on. When an event triggers, a POST will be made to the callback URL with a payload
    of notification information. Available resources and their events include ''CccCampaign'':
    [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'', ''stopped'',
    ''finished''], ''TextBroadcast'': [''started'', ''stopped'', ''finished''], ''OutboundCall'':
    [''finished''], ''InboundCall'': [''finished''], ''OutboundText'': [''finished''],
    ''InboundText'': [''finished''], ''ContactList'': [''validationFinished'', ''validationFailed''].
    Webhooks support secret token which is used as signing key to HmacSHA1 hash of
    json payload which is returned in ''X-CallFire-Signature'' header. This header
    can be used to verify callback POST is coming from CallFire. See [security guide](https://developers.callfire.com/security-guide.html)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks
  tags: Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooks-post-openapi.md
- name: Callfire Find webhook resources
  x-api-slug: callfire
  description: 'Searches for webhook resources. Available resources include ''CccCampaign'':
    [''started'', ''stopped'', ''finished''], ''CallBroadcast'': [''started'', ''stopped'',
    ''finished''], ''TextBroadcast'': [''started'', ''stopped'', ''finished''], ''OutboundCall'':
    [''finished''], ''InboundCall'': [''finished''], ''OutboundText'': [''finished''],
    ''InboundText'': [''finished''], ''ContactList'': [''validationFinished'', ''validationFailed'']'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks/resources
  tags: Webhooks,Resources
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooksresources-get-openapi.md
- name: Callfire Find specific webhook resource
  x-api-slug: callfire
  description: Returns information about supported events for a given webhook resource
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks/resources/{resource}
  tags: Webhooks,Resources,Resource
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooksresourcesresource-get-openapi.md
- name: Callfire Delete a webhook
  x-api-slug: callfire
  description: Deletes a webhook instance. Will be removed permanently
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks/{id}
  tags: Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooksid-delete-openapi.md
- name: Callfire Find a specific webhook
  x-api-slug: callfire
  description: Returns a single Webhook instance for a given webhook id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks/{id}
  tags: Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooksid-get-openapi.md
- name: Callfire Update a webhook
  x-api-slug: callfire
  description: Updates the information in existing webhook
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//webhooks/{id}
  tags: Webhooks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/webhooksid-put-openapi.md
- name: Callfire
  x-api-slug: callfire
  description: Grow your business with virtual phone numbers, IVR, voice broadcasting,
    mass text messaging services and power dialing. Try CallFire for FREE!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2
  tags: CallFire
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/callfire/master/_listings/callfire/openapi.md
x-common:
- type: x--net-sdk
  url: https://github.com/CallFire/CallFire-CSharp-SDK
- type: x-account-billing
  url: https://answers.callfire.com/hc/en-us/sections/200166268-Billing
- type: x-account-settings
  url: https://answers.callfire.com/hc/en-us/sections/200187056-Account-Settings
- type: x-authentication
  url: https://www.callfire.com/api-documentation/how-do-i-enable-api-on-my-account
- type: x-blog
  url: https://www.callfire.com/blog
- type: x-blog-rss
  url: https://www.callfire.com/blog/feed
- type: x-twitter
  url: https://twitter.com/CallFire
- type: x-case-studies
  url: https://www.callfire.com/case-studies
- type: x-compliance
  url: https://www.callfire.com/legal/compliance
- type: x-contact-form
  url: https://www.callfire.com/contact
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/callfire
- type: x-crunchbase
  url: https://crunchbase.com/organization/callfire
- type: x-developer
  url: https://www.callfire.com/api-documentation
- type: x-documentation
  url: https://www.callfire.com/api-documentation/rest/version/1.1
- type: x-drupal-plugin
  url: https://github.com/CallFire/CallFire-Drupal-Integration
- type: x-email
  url: answers@callfire.com
- type: x-email
  url: support@callfire.com
- type: x-facebook
  url: https://www.facebook.com/callfire
- type: x-faq
  url: https://answers.callfire.com/hc/en-us/sections/200193833-FAQs
- type: x-getting-started
  url: https://www.callfire.com/help/docs/getting-started
- type: x-github
  url: https://github.com/callfire
- type: x-glossary
  url: https://www.callfire.com/help/glossary/communications
- type: x-google-plus
  url: https://plus.google.com/100142045997033051154
- type: x-messages
  url: https://www.callfire.com/ui/number/messages?6
- type: x-partners
  url: https://www.callfire.com/partners
- type: x-phone
  url: 1.877.897.3473
- type: x-php-sdk
  url: https://github.com/CallFire/CallFire-PHP-SDK
- type: x-pricing
  url: https://www.callfire.com/pricing
- type: x-privacy
  url: https://www.callfire.com/legal/privacy
- type: x-selfservice-registration
  url: https://www.callfire.com/ui/register?1
- type: x-terms-of-service
  url: https://www.callfire.com/legal/terms
- type: x-tickets
  url: https://answers.callfire.com/hc/en-us/requests/new
- type: x-tour
  url: javascript:;
- type: x-videos
  url: https://answers.callfire.com/hc/en-us/articles/200849247-Videos
- type: x-webinars
  url: https://answers.callfire.com/hc/en-us/articles/202174798-Webinars
- type: x-website
  url: http://www.callfire.com
- type: x-wordpress-plugin
  url: https://github.com/CallFire/CallFire-WordPress-Integration
- type: x-youtube
  url: https://www.youtube.com/user/CallFireTelephony
- type: x-zapier
  url: https://zapier.com/zapbook/callfire/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---