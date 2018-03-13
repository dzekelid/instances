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
  /?Action=RebootDBInstance&k=1:
    get:
      summary: Reboot D B Instance
      description: Rebooting a DB instance restarts the database engine service
      operationId: rebootdbinstance
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: ForceFailover
        description: When true, the reboot will be conducted through a MultiAZ failover
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