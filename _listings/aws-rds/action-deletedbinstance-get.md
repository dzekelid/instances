---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteDBInstance&k=1:
    get:
      summary: Delete D B Instance
      description: The DeleteDBInstance action deletes a previously provisioned DB
        instance
      operationId: deletedbinstance
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier for the DB instance to be deleted
        type: string
      - in: query
        name: FinalDBSnapshotIdentifier
        description: The DBSnapshotIdentifier of the new DBSnapshot created when SkipFinalSnapshot        is
          set to false
        type: string
      - in: query
        name: SkipFinalSnapshot
        description: Determines whether a final DB snapshot is created before the
          DB instance is deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - instances
definitions: []
x-collection-name: AWS RDS
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