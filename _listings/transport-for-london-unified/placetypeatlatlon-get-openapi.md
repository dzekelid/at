---
swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 0
info:
  title: Transport for London Unified Place type  At  Lat  Lon
  description: "Gets any places of the given type whose geography intersects the given
    latitude and longitude. in practice this means the place\r\n            must be
    polygonal e.g. a boroughboundary.."
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
  /Place/{type}/At/{Lat}/{Lon}:
    get:
      summary: Place type  At  Lat  Lon
      description: "Gets any places of the given type whose geography intersects the
        given latitude and longitude. in practice this means the place\r\n            must
        be polygonal e.g. a boroughboundary.."
      operationId: Place_GetAt
      x-api-path-slug: placetypeatlatlon-get
      parameters:
      - in: query
        name: lat
      - in: path
        name: Lat
      - in: query
        name: location.lat
      - in: query
        name: location.lon
      - in: query
        name: lon
      - in: path
        name: Lon
      - in: path
        name: type
        description: The place type (a valid list of place types can be obtained from
          the /Place/Meta/placeTypes endpoint)
      responses:
        200:
          description: OK
      tags:
      - Place
      - Type
      - ""
      - At
      - ""
      - Lat
      - ""
      - Lon
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