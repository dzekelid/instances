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
  /?Action=CreateDBInstanceReadReplica&k=1:
    get:
      summary: Create D B Instance Read Replica
      description: Creates a DB instance for a DB instance running MySQL, MariaDB,
        or PostgreSQL that acts as a Read Replica of a source DB instance
      operationId: createdbinstancereadreplica
      parameters:
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the Read Replica during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The Amazon EC2 Availability Zone that the Read Replica will be
          created in
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the Read Replica to snapshots of the
          Read Replica; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the Read Replica
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier of the Read Replica
        type: string
      - in: query
        name: DBSubnetGroupName
        description: Specifies a DB subnet group for the DB instance
        type: string
      - in: query
        name: Iops
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the Read Replica
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: OptionGroupName
        description: The option group the DB instance will be associated with
        type: string
      - in: query
        name: Port
        description: The port number that the DB instance uses for connections
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: SourceDBInstanceIdentifier
        description: The identifier of the DB instance that will act as the source
          for the Read Replica
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the Read Replica
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