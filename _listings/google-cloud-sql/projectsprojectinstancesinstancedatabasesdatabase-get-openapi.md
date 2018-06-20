---
swagger: "2.0"
x-collection-name: Google Cloud SQL
x-complete: 0
info:
  title: Google Cloud SQL API Get Projects Project Instances Instance Databases Database
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
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
    post:
      summary: Add Projects Project Instances Instance Backupruns
      description: Creates a new backup run on demand. This method is applicable only
        to Second Generation instances.
      operationId: sql.backupRuns.insert
      x-api-path-slug: projectsprojectinstancesinstancebackupruns-post
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
      - Backupruns
  /projects/{project}/instances/{instance}/backupRuns/{id}:
    delete:
      summary: Delete Projects Project Instances Instance Backupruns
      description: Deletes the backup taken by a backup run.
      operationId: sql.backupRuns.delete
      x-api-path-slug: projectsprojectinstancesinstancebackuprunsid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the Backup Run to delete
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
      - Backupruns
    get:
      summary: Get Projects Project Instances Instance Backupruns
      description: Retrieves a resource containing information about a backup run.
      operationId: sql.backupRuns.get
      x-api-path-slug: projectsprojectinstancesinstancebackuprunsid-get
      parameters:
      - in: path
        name: id
        description: The ID of this Backup Run
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
      - Backupruns
  /projects/{project}/instances/{instance}/clone:
    post:
      summary: Add Projects Project Instances Instance Clone
      description: Creates a Cloud SQL instance as a clone of the source instance.
        The API is not ready for Second Generation instances yet.
      operationId: sql.instances.clone
      x-api-path-slug: projectsprojectinstancesinstanceclone-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: The ID of the Cloud SQL instance to be cloned (source)
      - in: path
        name: project
        description: Project ID of the source as well as the clone Cloud SQL instance
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Clone
  /projects/{project}/instances/{instance}/createEphemeral:
    post:
      summary: Add Projects Project Instances Instance Createephemeral
      description: Generates a short-lived X509 certificate containing the provided
        public key and signed by a private key specific to the target instance. Users
        may use the certificate to authenticate as themselves when connecting to the
        database.
      operationId: sql.sslCerts.createEphemeral
      x-api-path-slug: projectsprojectinstancesinstancecreateephemeral-post
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
        description: Project ID of the Cloud SQL project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Project
      - Instances
      - Instance
      - Createephemeral
  /projects/{project}/instances/{instance}/databases:
    get:
      summary: Get Projects Project Instances Instance Databases
      description: Lists databases in the specified Cloud SQL instance.
      operationId: sql.databases.list
      x-api-path-slug: projectsprojectinstancesinstancedatabases-get
      parameters:
      - in: path
        name: instance
        description: Cloud SQL instance ID
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
      - Instance
      - Databases
    post:
      summary: Add Projects Project Instances Instance Databases
      description: Inserts a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.insert
      x-api-path-slug: projectsprojectinstancesinstancedatabases-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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
      - Databases
  /projects/{project}/instances/{instance}/databases/{database}:
    delete:
      summary: Delete Projects Project Instances Instance Databases Database
      description: Deletes a database from a Cloud SQL instance.
      operationId: sql.databases.delete
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
      parameters:
      - in: path
        name: database
        description: Name of the database to be deleted in the instance
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
      - Databases
      - Database
    get:
      summary: Get Projects Project Instances Instance Databases Database
      description: Retrieves a resource containing information about a database inside
        a Cloud SQL instance.
      operationId: sql.databases.get
      x-api-path-slug: projectsprojectinstancesinstancedatabasesdatabase-get
      parameters:
      - in: path
        name: database
        description: Name of the database in the instance
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
      - Databases
      - Database
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