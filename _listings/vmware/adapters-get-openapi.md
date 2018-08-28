---
swagger: "2.0"
x-collection-name: VMWare
x-complete: 0
info:
  title: VMWare vRealize Operations Get An Adapter Instance(s) of Type (Kind)
  description: 'TODO: Add Description'
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/adapters:
    get:
      summary: Get Adapter Instances
      description: 'TODO: Add Description'
      operationId: ApiAdaptersGet
      x-api-path-slug: apiadapters-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Adapters
  /api/adapters/617d20fd-536a-4bea-9f5e-4c01dd845ddc/monitoringstate/start:
    put:
      summary: Start an adapter instance
      description: |-
        Replace the UUID with the ID of the adapter instance you want to start
        This can be retrieved using Get Adapter Instances
      operationId: ApiAdapters617d20fd536a4bea9f5e4c01dd845ddcMonitoringstateStartPut
      x-api-path-slug: apiadapters617d20fd536a4bea9f5e4c01dd845ddcmonitoringstatestart-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Adapters
      - Start
  /adapters:
    get:
      summary: Get An Adapter Instance(s) of Type (Kind)
      description: 'TODO: Add Description'
      operationId: AdaptersGet
      x-api-path-slug: adapters-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: adapterKindKey
      responses:
        200:
          description: OK
      tags:
      - Adapters
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