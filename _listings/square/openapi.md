swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/items:
    post:
      summary: Creates an item and at least one variation for it.
      description: Creates an item and at least one variation for it.
      operationId: CreateItem
      x-api-path-slug: v1location-iditems-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - At
      - Least
      - Variationit
  /v1/{location_id}/modifier-lists:
    post:
      summary: Creates an item modifier list and at least one modifier option for
        it.
      description: Creates an item modifier list and at least one modifier option
        for it.
      operationId: CreateModifierList
      x-api-path-slug: v1location-idmodifierlists-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create a modifier list for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Item
      - Modifier
      - List
      - At
      - Least
      - Modifier
      - Optionit