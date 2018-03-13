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
  /?Action=PurchaseReservedDBInstancesOffering&k=1:
    get:
      summary: Purchase Reserved D B Instances Offering
      description: Purchases a reserved DB instance offering
      operationId: purchasereserveddbinstancesoffering
      parameters:
      - in: query
        name: DBInstanceCount
        description: The number of instances to reserve
        type: string
      - in: query
        name: ReservedDBInstanceId
        description: Customer-specified identifier to track this reservation
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The ID of the Reserved DB instance offering to purchase
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
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