---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Options Instances Instanceid Sparkproxy **
  description: Options instances instanceid sparkproxy **.
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
  /instances/{instanceId}:
    get:
      summary: Get Instances Instanceid
      description: Get instances instanceid.
      operationId: getInstanceUsingGET
      x-api-path-slug: instancesinstanceid-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
    delete:
      summary: Delete Instances Instanceid
      description: Delete instances instanceid.
      operationId: stopInstanceUsingDELETE
      x-api-path-slug: instancesinstanceid-delete
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
  /instances/{instanceId}/appattempts/{attemptId}/containers:
    get:
      summary: Get Instances Instanceid Appattempts Attemptid Containers
      description: Get instances instanceid appattempts attemptid containers.
      operationId: getInstanceAttemptContainersUsingGET
      x-api-path-slug: instancesinstanceidappattemptsattemptidcontainers-get
      parameters:
      - in: path
        name: attemptId
        description: attemptId
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Appattempts
      - Attemptid
      - Containers
  /instances/{instanceId}/config:
    get:
      summary: Get Instances Instanceid Config
      description: Get instances instanceid config.
      operationId: listInstanceConfigFileUsingGET
      x-api-path-slug: instancesinstanceidconfig-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Config
  /instances/{instanceId}/config/{fileName}:
    get:
      summary: Get Instances Instanceid Config Filename
      description: Get instances instanceid config filename.
      operationId: getInstanceConfigFileUsingGET
      x-api-path-slug: instancesinstanceidconfigfilename-get
      parameters:
      - in: path
        name: fileName
        description: fileName
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Config
      - Filename
  /instances/{instanceId}/containers:
    get:
      summary: Get Instances Instanceid Containers
      description: Get instances instanceid containers.
      operationId: getInstanceContainersUsingGET
      x-api-path-slug: instancesinstanceidcontainers-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
  /instances/{instanceId}/containers/{containerId}/logs:
    get:
      summary: Get Instances Instanceid Containers Containerid Logs
      description: Get instances instanceid containers containerid logs.
      operationId: getInstanceContainerLogsUsingGET
      x-api-path-slug: instancesinstanceidcontainerscontaineridlogs-get
      parameters:
      - in: path
        name: containerId
        description: containerId
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
      - Containerid
      - Logs
  /instances/{instanceId}/containers/{containerId}/logs/{logName}:
    get:
      summary: Get Instances Instanceid Containers Containerid Logs Logname
      description: Get instances instanceid containers containerid logs logname.
      operationId: getInstanceContainerLogContentsUsingGET
      x-api-path-slug: instancesinstanceidcontainerscontaineridlogslogname-get
      parameters:
      - in: path
        name: containerId
        description: containerId
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: length
        description: length
      - in: path
        name: logName
        description: logName
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Containers
      - Containerid
      - Logs
      - Logname
  /instances/{instanceId}/sparkproxy/**:
    get:
      summary: Get Instances Instanceid Sparkproxy **
      description: Get instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingGET
      x-api-path-slug: instancesinstanceidsparkproxy-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    head:
      summary: Head Instances Instanceid Sparkproxy **
      description: Head instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingHEAD
      x-api-path-slug: instancesinstanceidsparkproxy-head
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Head
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    post:
      summary: Post Instances Instanceid Sparkproxy **
      description: Post instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPOST
      x-api-path-slug: instancesinstanceidsparkproxy-post
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    put:
      summary: Put Instances Instanceid Sparkproxy **
      description: Put instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPUT
      x-api-path-slug: instancesinstanceidsparkproxy-put
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    delete:
      summary: Delete Instances Instanceid Sparkproxy **
      description: Delete instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingDELETE
      x-api-path-slug: instancesinstanceidsparkproxy-delete
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    options:
      summary: Options Instances Instanceid Sparkproxy **
      description: Options instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingOPTIONS
      x-api-path-slug: instancesinstanceidsparkproxy-options
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Options
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
    patch:
      summary: Patch Instances Instanceid Sparkproxy **
      description: Patch instances instanceid sparkproxy **.
      operationId: getInstanceSparkProxyUsingPATCH
      x-api-path-slug: instancesinstanceidsparkproxy-patch
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Sparkproxy
      - '**'
  /instances/{instanceId}/submit-logs:
    get:
      summary: Get Instances Instanceid Submit Logs
      description: Get instances instanceid submit logs.
      operationId: getSparkSubmitLogsUsingGET
      x-api-path-slug: instancesinstanceidsubmitlogs-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      - in: query
        name: length
        description: length
      - in: query
        name: offset
        description: offset
      responses:
        200:
          description: Successful response
      tags:
      - Instances
      - Instanceid
      - Submit
      - Logs
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