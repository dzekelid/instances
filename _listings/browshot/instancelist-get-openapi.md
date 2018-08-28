---
swagger: "2.0"
x-collection-name: Browshot
x-complete: 0
info:
  title: Browshot Get all instances
  description: Get all instances.
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /instance/info:
    get:
      summary: Get information about an instance
      description: Get information about an instance.
      operationId: GetInstanceInfo
      x-api-path-slug: instanceinfo-get
      parameters:
      - in: query
        name: id
        description: instance ID
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Info
  /instance/list:
    get:
      summary: Get all instances
      description: Get all instances.
      operationId: GetInstancesInfo
      x-api-path-slug: instancelist-get
      responses:
        200:
          description: OK
      tags:
      - Instance
      - List
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