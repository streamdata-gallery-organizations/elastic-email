---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 0
info:
  title: Elastic Email SMTP API Delete Existing Subscriber
  description: Delete Existing Subscriber
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  attachments/upload/:
    get:
      summary: Upload Attachment
      description: The upload attachment command is used to upload an attachment for
        sending.
      operationId: getAttachmentsUpload
      x-api-path-slug: attachmentsupload-get
      parameters:
      - in: query
        name: api_key
        description: your api key
      - in: query
        name: file
        description: The file name being uploaded
      - in: query
        name: username
        description: username
      responses:
        200:
          description: OK
      tags:
      - Attachments
      - Upload
  lists/add-contact:
    get:
      summary: Add Existing Subscriber To List
      description: Add Existing Subscriber To List
      operationId: getListsAddContact
      x-api-path-slug: listsaddcontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to add subscriber to (separate by semi-colon
          to add to multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Add
      - Contact
  lists/create-contact:
    get:
      summary: Create New Subscriber
      description: Create New Subscriber
      operationId: getListsCreateContact
      x-api-path-slug: listscreatecontact-get
      parameters:
      - in: query
        name: api_key
        description: your api key found on the Account screen
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: the zip or postal code of the subscriber
        description: Your user name
      - in: query
        name: title
        description: the title for the subscriber (Mr
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Contact
  lists/create-lists:
    get:
      summary: Create New List
      description: Create New List
      operationId: getListsCreateLists
      x-api-path-slug: listscreatelists-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to create
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Lists
  lists/delete:
    get:
      summary: Delete Existing List
      description: Delete Existing List
      operationId: getListsDelete
      x-api-path-slug: listsdelete-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to delete
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
  lists/delete-contact:
    get:
      summary: Delete Existing Subscriber
      description: Delete Existing Subscriber
      operationId: getListsDeleteContact
      x-api-path-slug: listsdeletecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: email
        description: email address of subscriber/recipient (separate by semi-colon
          to remove multiple)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
      - Contact
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