---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve a backup_instance by backup_instance_id
  description: Only backup_instances you have permission to view will be returned
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_instances:
    get:
      summary: Retrieves a list of backup_instances associated with the specified
        backup_definition
      description: It is only possible to retrieve backup_instances for customers
        you are authorized to access. Records are returned in ascending order (by
        id), with a default of 20 per page. Links to the next, previous, first, and
        last pages can be found in the response headers.
      operationId: getV1BackupInstances
      x-api-path-slug: v1backup-instances-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: query
        name: backup_definition_id
        description: ID of the backup_definition to retrieve backup_instances for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
    post:
      summary: Create a new backup_instance from the specified backup_definition for
        the specified customer
      description: Create a new backup_instance from the specified backup_definition
        for the specified customer.
      operationId: postV1BackupInstances
      x-api-path-slug: v1backup-instances-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_instance[backup_definition_id]
        description: ID of the backup_definition to create a backup_instance for
      - in: formData
        name: backup_instance[backup_frequency]
        description: Frequency with which scheduled backups are performed
      - in: formData
        name: backup_instance[customer_id]
        description: ID of the customer to create the backup_instance for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
  /v1/backup_instances/{backup_instance_id}:
    get:
      summary: Retrieve a backup_instance by backup_instance_id
      description: Only backup_instances you have permission to view will be returned
      operationId: getV1BackupInstancesBackupInstance
      x-api-path-slug: v1backup-instancesbackup-instance-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
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