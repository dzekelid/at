swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/cache/{itemKey}:
    delete:
      summary: Deletes the item stored at {itemKey}
      description: Deletes the item stored at {itemkey}.
      operationId: Cache_DeleteItemByitemKey
      x-api-path-slug: apicacheitemkey-delete
      parameters:
      - in: path
        name: itemKey
        description: The item key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Item
      - Stored
      - At
      - ItemKey
  /api/progression/lettings/withdrawInstruction:
    post:
      summary: Withdraw a letting at the end of let
      description: Withdraw a letting at the end of let.
      operationId: LettingsProgression_WithdrawInstructionBylettingInstructionCommandData
      x-api-path-slug: apiprogressionlettingswithdrawinstruction-post
      parameters:
      - in: body
        name: lettingInstructionCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Letting
      - At
      - End
      - Of
      - Let
  /api/progression/lettings/completeletting:
    post:
      summary: Withdraw a letting at the end of let
      description: Withdraw a letting at the end of let.
      operationId: LettingsProgression_CompleteLettingBycompleteCommandData
      x-api-path-slug: apiprogressionlettingscompleteletting-post
      parameters:
      - in: body
        name: completeCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Withdraw
      - Letting
      - At
      - End
      - Of
      - Let