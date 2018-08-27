swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
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
  /school/districtdetail:
    get:
      summary: Return details about a particular school district.
      description: Search by district number to return all of the available details
        about a school district
      operationId: propertySchoolDistrictDetail
      x-api-path-slug: schooldistrictdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: district number
      responses:
        200:
          description: OK
      tags:
      - Return
      - Details
      - About
      - Particular
      - School
      - District