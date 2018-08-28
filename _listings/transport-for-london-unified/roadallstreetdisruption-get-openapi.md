---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Road all  Street  Disruption
  description: Gets a list of disrupted streets. if no date filters are provided,
    current disruptions are returned..
  version: v1
host: api.tfl.gov.uk
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Place/Address/Streets/{Postcode}:
    get:
      summary: Place  Address  Streets  Postcode
      description: Gets the set of streets associated with a post code..
      operationId: Place_GetStreetsByPostCode
      x-api-path-slug: placeaddressstreetspostcode-get
      parameters:
      - in: query
        name: postcode
      - in: path
        name: Postcode
      - in: query
        name: postcodeInput.postcode
      responses:
        200:
          description: OK
      tags:
      - Place
      - ""
      - Ress
      - ""
      - Streets
      - ""
      - Code
  /Road/all/Street/Disruption:
    get:
      summary: Road all  Street  Disruption
      description: Gets a list of disrupted streets. if no date filters are provided,
        current disruptions are returned..
      operationId: Road_DisruptedStreets
      x-api-path-slug: roadallstreetdisruption-get
      parameters:
      - in: query
        name: endDate
        description: Optional, The end time to filter on
      - in: query
        name: startDate
        description: Optional, the start time to filter on
      responses:
        200:
          description: OK
      tags:
      - Road
      - ""
      - ""
      - Street
      - ""
      - Disruption
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