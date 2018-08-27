swagger: "2.0"
x-collection-name: Transport for London Unified
x-complete: 1
info:
  title: Transport for London Unified
  description: our-unified-api-brings-together-data-across-all-modes-of-transport-into-a-single-restful-api--this-api-provides-access-to-the-most-highly-requested-realtime-and-status-infomation-across-all-the-modes-of-transport-in-a-single-and-consistent-way--access-to-the-developer-documentation-is-available-at-httpsapi-tfl-gov-uk
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