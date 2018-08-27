swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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