---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Get Instances
  description: Get instances.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/service_instances/{instanceId}:
    put:
      summary: Put Service Instances
      description: Put service instances.
      operationId: putV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-put
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
    delete:
      summary: Delete Service Instances
      description: Delete service instances.
      operationId: deleteV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-delete
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: plan_id
        description: plan_id
      - in: query
        name: service_id
        description: service_id
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
    patch:
      summary: Patch Service Instances
      description: Patch service instances.
      operationId: patchV2ServiceInstancesInstance
      x-api-path-slug: v2service-instancesinstanceid-patch
      parameters:
      - in: query
        name: accepts_incomplete
        description: accepts_incomplete
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
  /v2/service_instances/{instanceId}/last_operation:
    get:
      summary: Get Service Instances Last Operation
      description: Get service instances last operation.
      operationId: getV2ServiceInstancesInstanceLastOperation
      x-api-path-slug: v2service-instancesinstanceidlast-operation-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Last
      - Operation
  /v2/service_instances/{instanceId}/service_bindings/{bindingId}:
    put:
      summary: Put Service Instances Service Bindings Bindingid
      description: Put service instances service bindings bindingid.
      operationId: putV2ServiceInstancesInstanceServiceBindingsBinding
      x-api-path-slug: v2service-instancesinstanceidservice-bindingsbindingid-put
      parameters:
      - in: path
        name: bindingId
        description: bindingId
      - in: path
        name: instanceId
        description: instanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Service
      - Bindings
      - Bindingid
    delete:
      summary: Delete Service Instances Service Bindings Bindingid
      description: Delete service instances service bindings bindingid.
      operationId: deleteV2ServiceInstancesInstanceServiceBindingsBinding
      x-api-path-slug: v2service-instancesinstanceidservice-bindingsbindingid-delete
      parameters:
      - in: path
        name: bindingId
        description: bindingId
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: plan_id
        description: plan_id
      - in: query
        name: service_id
        description: service_id
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Service
      - Bindings
      - Bindingid
  /instances:
    get:
      summary: Get Instances
      description: Get instances.
      operationId: findInstancesUsingGET
      x-api-path-slug: instances-get
      parameters:
      - in: query
        name: flowName
        description: flowName
      - in: query
        name: maxUpdateTime
        description: maxUpdateTime
      - in: query
        name: minUpdateTime
        description: minUpdateTime
      - in: query
        name: name
        description: name
      - in: query
        name: page
        description: Results page you want to retrieve (0
      - in: query
        name: size
        description: Number of records per page
      - in: query
        name: sort
        description: 'Sorting criteria in the format: property(,asc|desc)'
      - in: query
        name: statuses
        description: statuses
      - in: query
        name: tag
        description: tag
      - in: query
        name: type
        description: type
      responses:
        200:
          description: Successful response
      tags:
      - Instances
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