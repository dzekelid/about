---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Return details about a particular school.
  description: Search by school ID to return all of the available details about a
    school
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /school/detail:
    get:
      summary: Return details about a particular school.
      description: Search by school ID to return all of the available details about
        a school
      operationId: propertyDetails
      x-api-path-slug: schooldetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: school id
      responses:
        200:
          description: OK
      tags:
      - Return
      - Details
      - About
      - Particular
      - School
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