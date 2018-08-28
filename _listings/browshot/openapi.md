swagger: "2.0"
x-collection-name: Browshot
x-complete: 1
info:
  title: Browshot
  description: take-screenshots-of-any-website-in-real-time
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