---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 0
info:
  title: Google Cloud SQL API Get Projects Project Instances Instance Backupruns
  description: Lists all backup runs associated with a given instance and configuration
    in the reverse chronological order of the enqueued time.
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances:
    get:
      summary: Get Projects Project Instances
      description: Lists instances under a given project in the alphabetical order
        of the instance name.
      operationId: sql.instances.list
      x-api-path-slug: projectsprojectinstances-get
      parameters:
      - in: query
        name: filter
        description: A filter expression for filtering listed instances
      - in: query
        name: maxResults
        description: The maximum number of results to return per response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: path
        name: project
        description: Project ID of the project for which to list Cloud SQL instances
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
    post:
      summary: Add Projects Project Instances
      description: Creates a new Cloud SQL instance.
      operationId: sql.instances.insert
      x-api-path-slug: projectsprojectinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID of the project to which the newly created Cloud SQL
          instances should belong
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
  /projects/{project}/instances/{instance}:
    delete:
      summary: Delete Projects Project Instances Instance
      description: Deletes a Cloud SQL instance.
      operationId: sql.instances.delete
      x-api-path-slug: projectsprojectinstancesinstance-delete
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance to be deleted
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    get:
      summary: Get Projects Project Instances Instance
      description: Retrieves a resource containing information about a Cloud SQL instance.
      operationId: sql.instances.get
      x-api-path-slug: projectsprojectinstancesinstance-get
      parameters:
      - in: path
        name: instance
        description: Database instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    patch:
      summary: Patch Projects Project Instances Instance
      description: 'Updates settings of a Cloud SQL instance. Caution: This is not
        a partial update, so you must include values for all the settings that you
        want to retain. For partial updates, use patch.. This method supports patch
        semantics.'
      operationId: sql.instances.patch
      x-api-path-slug: projectsprojectinstancesinstance-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
    put:
      summary: Put Projects Project Instances Instance
      description: 'Updates settings of a Cloud SQL instance. Caution: This is not
        a partial update, so you must include values for all the settings that you
        want to retain. For partial updates, use patch.'
      operationId: sql.instances.update
      x-api-path-slug: projectsprojectinstancesinstance-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Put
      - Projects
      - Project
      - Instances
      - Instance
  /projects/{project}/instances/{instance}/backupRuns:
    get:
      summary: Get Projects Project Instances Instance Backupruns
      description: Lists all backup runs associated with a given instance and configuration
        in the reverse chronological order of the enqueued time.
      operationId: sql.backupRuns.list
      x-api-path-slug: projectsprojectinstancesinstancebackupruns-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
      - in: query
        name: maxResults
        description: Maximum number of backup runs per response
      - in: query
        name: pageToken
        description: A previously-returned page token representing part of the larger
          set of results to view
      - in: path
        name: project
        description: Project ID of the project that contains the instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Backupruns
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