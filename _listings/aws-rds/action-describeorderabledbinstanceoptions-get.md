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
  /?Action=DescribeOrderableDBInstanceOptions&k=1:
    get:
      summary: Describe Orderable D B Instance Options
      description: Returns a list of orderable DB instance options for the specified
        engine
      operationId: describeorderabledbinstanceoptions
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Engine
        description: The name of the engine to retrieve DB instance options for
        type: string
      - in: query
        name: EngineVersion
        description: The engine version filter value
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: LicenseModel
        description: The license model filter value
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeOrderableDBInstanceOptions
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: Vpc
        description: The VPC filter value
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