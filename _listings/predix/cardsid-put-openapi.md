---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Views Update attributes for a Card instance and persist it.
  version: 1.0.0
  description: Update attributes for a card instance and persist it..
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
  /v1/proxy/resource:
    get:
      summary: retrieve service instance
      description: API to retrieve service instance
      operationId: retrieveUsingGET
      x-api-path-slug: v1proxyresource-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Service
      - Instance
  /v1/tenant/{tenantName}/service/{instanceName}:
    put:
      summary: update a PROVISIONED service instance
      description: Update a provisioned service instance.
      operationId: updateServiceUsingPUT
      x-api-path-slug: v1tenanttenantnameserviceinstancename-put
      parameters:
      - in: path
        name: instanceName
        description: instanceName
      - in: header
        name: Predix-Zone-Id
      - in: body
        name: serviceRequest
        description: serviceRequest
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenantName
        description: tenantName
      responses:
        200:
          description: Successful response
      tags:
      - Update
      - PROVISIONED
      - Service
      - Instance
  /v1/tenant/{tenantName}/service/{serviceName}:
    delete:
      summary: Delete service instance
      description: Delete service instance.
      operationId: deleteServiceInstanceUsingDELETE
      x-api-path-slug: v1tenanttenantnameserviceservicename-delete
      parameters:
      - in: query
        name: instanceName
        description: instanceName
      - in: header
        name: Predix-Zone-Id
      - in: path
        name: serviceName
        description: serviceName
      - in: path
        name: tenantName
        description: tenantName
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instance
  /decks:
    get:
      summary: Find all instances of the Deck matched by filter.
      description: Find all instances of the deck matched by filter..
      operationId: getDecks
      x-api-path-slug: decks-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Deck
      - Matched
      - By
      - Filter
    post:
      summary: Create a new instance of the Deck and persist it.
      description: Create a new instance of the deck and persist it..
      operationId: postDecks
      x-api-path-slug: decks-post
      parameters:
      - in: body
        name: data
        description: Deck instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Deck
      - Persist
      - It
  /cards:
    get:
      summary: Find all instances of the Card matched by filter.
      description: Find all instances of the card matched by filter..
      operationId: getCards
      x-api-path-slug: cards-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields, where, include, order, offset, and limit
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Instances
      - Of
      - Card
      - Matched
      - By
      - Filter
    post:
      summary: Create a new instance of the Cards and persist it.
      description: Create a new instance of the cards and persist it..
      operationId: postCards
      x-api-path-slug: cards-post
      parameters:
      - in: body
        name: data
        description: Card instance data
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Instance
      - Of
      - Cards
      - Persist
      - It
  /decks/{id}/tags:
    post:
      summary: Creates a new instance in tags of this Tag.
      description: Creates a new instance in tags of this tag..
      operationId: postDecksTags
      x-api-path-slug: decksidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Tag
  /decks/{id}:
    get:
      summary: Find a Deck instance by id.
      description: Find a deck instance by id..
      operationId: getDecks
      x-api-path-slug: decksid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Deck id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Deck
      - Instance
      - By
      - Id
    delete:
      summary: Delete a Tag instance by id.
      description: Delete a tag instance by id..
      operationId: deleteDecks
      x-api-path-slug: decksid-delete
      parameters:
      - in: path
        name: id
        description: Deck id
      responses:
        200:
          description: OK
      tags:
      - Tag
      - Instance
      - By
      - Id
    put:
      summary: Update attributes for a Tag instance and persist it.
      description: Update attributes for a tag instance and persist it..
      operationId: putDecks
      x-api-path-slug: decksid-put
      parameters:
      - in: body
        name: data
        description: An object of Deck property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Tag
      - Instance
      - Persist
      - It
  /cards/{id}/tags:
    post:
      summary: Creates a new instance in tags of this Card.
      description: Creates a new instance in tags of this card..
      operationId: postCardsTags
      x-api-path-slug: cardsidtags-post
      parameters:
      - in: body
        name: data
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Instance
      - In
      - Tags
      - Of
      - This
      - Card
  /cards/{id}:
    get:
      summary: Find a Card instance by id.
      description: Find a card instance by id..
      operationId: getCards
      x-api-path-slug: cardsid-get
      parameters:
      - in: query
        name: filter
        description: Filter defining fields and include
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Card
      - Instance
      - By
      - Id
    delete:
      summary: Delete a Card instance by id.
      description: Delete a card instance by id..
      operationId: deleteCards
      x-api-path-slug: cardsid-delete
      parameters:
      - in: path
        name: id
        description: Card id
      responses:
        200:
          description: OK
      tags:
      - Card
      - Instance
      - By
      - Id
    put:
      summary: Update attributes for a Card instance and persist it.
      description: Update attributes for a card instance and persist it..
      operationId: putCards
      x-api-path-slug: cardsid-put
      parameters:
      - in: body
        name: data
        description: An object of Card property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Card
      - Instance
      - Persist
      - It
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