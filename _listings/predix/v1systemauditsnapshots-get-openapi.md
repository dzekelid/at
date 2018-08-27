---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Assets Get a snapshot of an entity at or before a specified datetime
    (ISO-8601).
  description: For detailed documentation of all available query options please refer
    to Predix Asset Documentation.
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/system/audit/snapshots:
    get:
      summary: Get a snapshot of an entity at or before a specified datetime (ISO-8601).
      description: For detailed documentation of all available query options please
        refer to Predix Asset Documentation.
      operationId: getV1SystemAuditSnapshots
      x-api-path-slug: v1systemauditsnapshots-get
      parameters:
      - in: query
        name: filter
        description: identifier={entity uri}:{before|eBefore}={ISO-8601 datetime}
      responses:
        200:
          description: Successful response
      tags:
      - Snapshot
      - Of
      - Entity
      - At
      - Before
      - Specified
      - Datetime
      - (ISO-8601)
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