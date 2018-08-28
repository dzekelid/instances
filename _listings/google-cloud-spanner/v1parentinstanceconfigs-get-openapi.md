---
swagger: "2.0"
x-collection-name: Google Cloud Spanner
x-complete: 0
info:
  title: Google Cloud Spanner API Get Instance Configurations
  description: Lists the supported instance configurations for a given project.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: spanner.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    patch:
      summary: Update Instance
      description: |-
        Updates an instance, and begins allocating or releasing resources
        as requested. The returned long-running
        operation can be used to track the
        progress of updating the instance. If the named instance does not
        exist, returns `NOT_FOUND`.

        Immediately upon completion of this request:

          * For resource types for which a decrease in the instance's allocation
            has been requested, billing is based on the newly-requested level.

        Until completion of the returned operation:

          * Cancelling the operation sets its metadata's
            cancel_time, and begins
            restoring resources to their pre-request values. The operation
            is guaranteed to succeed at undoing all resource changes,
            after which point it terminates with a `CANCELLED` status.
          * All other attempts to modify the instance are rejected.
          * Reading the instance via the API continues to give the pre-request
            resource levels.

        Upon completion of the returned operation:

          * Billing begins for all successfully-allocated resources (some types
            may have lower than the requested levels).
          * All newly-reserved resources are available for serving the instance's
            tables.
          * The instance's new resource levels are readable via the API.

        The returned long-running operation will
        have a name of the format `<instance_name>/operations/<operation_id>` and
        can be used to track the instance modification.  The
        metadata field type is
        UpdateInstanceMetadata.
        The response field type is
        Instance, if successful.

        Authorization requires `spanner.instances.update` permission on
        resource name.
      operationId: spanner.projects.instances.patch
      x-api-path-slug: v1name-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{name}:cancel:
    post:
      summary: Cancel Instance
      description: |-
        Starts asynchronous cancellation on a long-running operation.  The server
        makes a best effort to cancel the operation, but success is not
        guaranteed.  If the server doesn't support this method, it returns
        `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
        Operations.GetOperation or
        other methods to check whether the cancellation succeeded or whether the
        operation completed despite cancellation. On successful cancellation,
        the operation is not deleted; instead, it becomes an operation with
        an Operation.error value with a google.rpc.Status.code of 1,
        corresponding to `Code.CANCELLED`.
      operationId: spanner.projects.instances.databases.operations.cancel
      x-api-path-slug: v1namecancel-post
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{parent}/instanceConfigs:
    get:
      summary: Get Instance Configurations
      description: Lists the supported instance configurations for a given project.
      operationId: spanner.projects.instanceConfigs.list
      x-api-path-slug: v1parentinstanceconfigs-get
      parameters:
      - in: query
        name: pageSize
        description: Number of instance configurations to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_tokenfrom
          a previous ListInstanceConfigsResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
  /v1/{parent}/instances:
    get:
      summary: Get Instances
      description: Lists all instances in the given project.
      operationId: spanner.projects.instances.list
      x-api-path-slug: v1parentinstances-get
      parameters:
      - in: query
        name: filter
        description: An expression for filtering the results of the request
      - in: query
        name: pageSize
        description: Number of instances to be returned in the response
      - in: query
        name: pageToken
        description: If non-empty, `page_token` should contain anext_page_token from
          aprevious ListInstancesResponse
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
    post:
      summary: Create instance
      description: |-
        Creates an instance and begins preparing it to begin serving. The
        returned long-running operation
        can be used to track the progress of preparing the new
        instance. The instance name is assigned by the caller. If the
        named instance already exists, `CreateInstance` returns
        `ALREADY_EXISTS`.

        Immediately upon completion of this request:

          * The instance is readable via the API, with all requested attributes
            but no allocated resources. Its state is `CREATING`.

        Until completion of the returned operation:

          * Cancelling the operation renders the instance immediately unreadable
            via the API.
          * The instance can be deleted.
          * All other attempts to modify the instance are rejected.

        Upon completion of the returned operation:

          * Billing for all successfully-allocated resources begins (some types
            may have lower than the requested levels).
          * Databases can be created in the instance.
          * The instance's allocated resource levels are readable via the API.
          * The instance's state becomes `READY`.

        The returned long-running operation will
        have a name of the format `<instance_name>/operations/<operation_id>` and
        can be used to track creation of the instance.  The
        metadata field type is
        CreateInstanceMetadata.
        The response field type is
        Instance, if successful.
      operationId: spanner.projects.instances.create
      x-api-path-slug: v1parentinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: parent
        description: Required
      responses:
        200:
          description: OK
      tags:
      - Instance
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