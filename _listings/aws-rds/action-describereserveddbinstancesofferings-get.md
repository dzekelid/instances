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
  /?Action=DescribeReservedDBInstancesOfferings&k=1:
    get:
      summary: Describe Reserved D B Instances Offerings
      description: Lists available reserved DB instance offerings
      operationId: describereserveddbinstancesofferings
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Duration
        description: Duration filter value, specified in years or seconds
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: MultiAZ
        description: The Multi-AZ filter value
        type: string
      - in: query
        name: OfferingType
        description: The offering type filter value
        type: string
      - in: query
        name: ProductDescription
        description: Product description filter value
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The offering identifier filter value
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