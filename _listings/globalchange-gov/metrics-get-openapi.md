---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get overall metrics about GCIS data
  description: Get overall metrics about GCIS data
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics:
    get:
      summary: Get overall metrics about GCIS data
      description: Get overall metrics about GCIS data
      operationId: get-overall-metrics-about-gcis-data
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - Overall
      - Metrics
      - About
      - GCIS
      - Data
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