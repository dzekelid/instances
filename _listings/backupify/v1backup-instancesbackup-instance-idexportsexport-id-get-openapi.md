---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve a specific export for the specified backup_instance
  description: You can only retrieve exports for backup_instances you have access
    to
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
    put:
      summary: Modify the specified backup_instance
      description: Only backup_instances you have permission to change can be modified
      operationId: putV1BackupInstancesBackupInstance
      x-api-path-slug: v1backup-instancesbackup-instance-id-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: formData
        name: backup_instance[backup_frequency]
        description: Frequency with which scheduled backups will be performed
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
  /v1/backup_instances/{backup_instance_id}/backups:
    get:
      summary: Retrieve a list of all backups for the specified backup_instance.
      description: Only backups belonging to backup_instances you have permission
        to manage can be retrieved. Records are returned in ascending order (by id),
        with a default of 20 per page. Links to the next, previous, first, and last
        pages can be found in the response headers.
      operationId: getV1BackupInstancesBackupInstanceBackups
      x-api-path-slug: v1backup-instancesbackup-instance-idbackups-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to backup
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
      - Backups
    post:
      summary: Perform an immediate backup of the specified backup_instance
      description: Only backup_instances you have permission to manage can be backed
        up
      operationId: postV1BackupInstancesBackupInstanceBackups
      x-api-path-slug: v1backup-instancesbackup-instance-idbackups-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to backup
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
      - Backups
  /v1/backup_instances/{backup_instance_id}/backups/active:
    get:
      summary: Retrieve the active backup for the specified backup_instance if one
        exists
      description: Only backups belonging to backup_instances you have permission
        to access can be retrieved
      operationId: getV1BackupInstancesBackupInstanceBackupsActive
      x-api-path-slug: v1backup-instancesbackup-instance-idbackupsactive-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance the requested backup belongs to
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
      - Backups
      - Active
  /v1/backup_instances/{backup_instance_id}/backups/{backup_id}:
    get:
      summary: Retrieve the specified backup for the specified backup_instance
      description: Only backups belonging to backup_instances you have permission
        to access can be retrieved
      operationId: getV1BackupInstancesBackupInstanceBackupsBackup
      x-api-path-slug: v1backup-instancesbackup-instance-idbackupsbackup-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_id
        description: ID of the backup to retrieve
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance the requested backup belongs to
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
      - Backups
      - Backup
      - Id
  /v1/backup_instances/{backup_instance_id}/endpoints:
    get:
      summary: Retrieve a list of endpoints for the specified backup_instance
      description: You can only retrieve endpoints for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceEndpoints
      x-api-path-slug: v1backup-instancesbackup-instance-idendpoints-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
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
      - Endpoints
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}:
    get:
      summary: Retrieve a specific endpoint by name for the specified backup_instance
      description: You can only retrieve endpoints for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointName
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-name-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve as defined by the backup_definition
          of the specified backup_instance
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
      - Endpoints
      - Endpoint
      - Name
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records:
    get:
      summary: Retrieve a list of records stored for the specified endpoint and backup_instance
      description: You can only retrieve records for endpoints that belong to backup_instances
        you have access to. Records are returned in ascending order (by id), with
        a default of 20 per page. Links to the next, previous, first, and last pages
        can be found in the response headers.
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecords
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecords-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: ID of the endpoint to retrieve records for
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
      - Endpoints
      - Endpoint
      - Name
      - Records
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records/{record_id}:
    get:
      summary: Retrieve a specific record by id for the specified endpoint and backup_instance
      description: You can only retrieve records for endpoints of backup_instances
        you have access to
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecord
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecordsrecord-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve the record from
      - in: path
        name: record_id
        description: The id of the endpoint record to retrieve
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
      - Endpoints
      - Endpoint
      - Name
      - Records
      - Record
      - Id
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records/{record_id}/blob:
    get:
      summary: Retrieve the blob associated with the specified record for the specified
        endpoint and backup_instance
      description: Retrieve the blob associated with the specified record for the
        specified endpoint and backup_instance.
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecordBlob
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecordsrecord-idblob-get
      parameters:
      - in: header
        name: Access-Token
        description: Access Token granted from client credentials authorizing vendor
          to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve the record from
      - in: path
        name: record_id
        description: The id of the endpoint record the blob belongs to
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
      - Endpoints
      - Endpoint
      - Name
      - Records
      - Record
      - Id
      - Blob
  /v1/backup_instances/{backup_instance_id}/exports:
    get:
      summary: Retrieve a list of exports for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve exports for
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
      - Exports
    post:
      summary: Perform an export of the most recent backup of the specified backup_instance
      description: Perform an export of the most recent backup of the specified backup_instance.
      operationId: postV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to export
      - in: formData
        name: export_run[backup_run_id]
        description: ID of a specific backup_run to export
      - in: formData
        name: export_run[content_types]
        description: Comma separated list of blob content-types to export
      - in: formData
        name: export_run[export_datetime]
        description: 'Date (format: YYYY-MM-DD) from which to export'
      - in: formData
        name: export_run[export_formats]
        description: Comma separated list of export format options
      - in: formData
        name: export_run[force_full]
        description: Flag to force a full export, as opposed to re-authorizing an
          old export if the data is the same
      - in: formData
        name: export_run[send_confirmation]
        description: Flag to send a confirmation email w/export link upon completion
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
      - Exports
  /v1/backup_instances/{backup_instance_id}/exports/{export_id}:
    get:
      summary: Retrieve a specific export for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceExportsExport
      x-api-path-slug: v1backup-instancesbackup-instance-idexportsexport-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an export for
      - in: path
        name: export_id
        description: ID of the export to retrieve
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
      - Exports
      - Export
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