---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Applications Application  Instances. Format
  version: 1.0.0
  description: "This API endpoint returns a \npaginated list of instances associated
    with the given application. The time range for summary data is the last 10 minutes.\n\nApplication
    instances can be filtered by hostname, or the list of application instance IDs.\n\nSee
    our documentation for a discussion and examples of\nusing  filters \nand summary
    data output."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /applications/{application_id}/instances.{format}:
    get:
      summary: Get Applications Application  Instances. Format
      description: "This API endpoint returns a \npaginated list of instances associated
        with the given application. The time range for summary data is the last 10
        minutes.\n\nApplication instances can be filtered by hostname, or the list
        of application instance IDs.\n\nSee our documentation for a discussion and
        examples of\nusing  filters \nand summary data output."
      operationId: getApplicationsApplicationInstances.Format
      x-api-path-slug: applicationsapplication-idinstances-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: filter[hostname]
        description: Filter by server hostname
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application instance ids
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances.
      - Format
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