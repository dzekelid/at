---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets all employers at the specified effective date
  description: Gets links to all employers contained under the authorised application
    scope for the specified effective date.
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/Employees/{EffectiveDate}:
    get:
      summary: Get employees from employer at a given effective date.
      description: Get links to all employees for the employer on specified effective
        date.
      operationId: GetEmployeesByEffectiveDate
      x-api-path-slug: employeremployeridemployeeseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/Pensions/{EffectiveDate}:
    get:
      summary: Get pensions from employer at a given effective date.
      description: Get links to all pensions for the employer on specified effective
        date.
      operationId: GetPensionsByEffectiveDate
      x-api-path-slug: employeremployeridpensionseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pensions
      - From
      - Employer
      - At
      - Given
      - Effective
      - Date
  /Employer/{EmployerId}/{EffectiveDate}:
    get:
      summary: Gets the employer at the specified effective
      description: Returns the employer's state at the specified effective date.
      operationId: GetEmployerByEffectiveDate
      x-api-path-slug: employeremployerideffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employer
      - At
      - Specified
      - Effective
  /Employers/{EffectiveDate}:
    get:
      summary: Gets all employers at the specified effective date
      description: Gets links to all employers contained under the authorised application
        scope for the specified effective date.
      operationId: GetEmployersByEffectiveDate
      x-api-path-slug: employerseffectivedate-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EffectiveDate
        description: The effective date to be applied
      responses:
        200:
          description: OK
      tags:
      - ""
      - Employers
      - At
      - Specified
      - Effective
      - Date
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