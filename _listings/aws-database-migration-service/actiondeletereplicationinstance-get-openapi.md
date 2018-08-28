---
swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 0
info:
  title: AWS Database Migration Service API Delete Replication Instance
  version: 1.0.0
  description: Deletes the specified replication instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeOrderableReplicationInstances:
    get:
      summary: Describe Orderable Replication Instances
      description: Returns information about the replication instance types that can
        be created in the specified region.
      operationId: describeOrderableReplicationInstances
      x-api-path-slug: actiondescribeorderablereplicationinstances-get
      parameters:
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DescribeReplicationInstances:
    get:
      summary: Describe Replication Instances
      description: Returns information about replication instances for your account
        in the current region.
      operationId: describeReplicationInstances
      x-api-path-slug: actiondescribereplicationinstances-get
      parameters:
      - in: query
        name: Filters
        description: Filters applied to the describe action
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous      request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=CreateReplicationInstance:
    get:
      summary: Create Replication Instance
      description: Creates the replication instance using the specified parameters.
      operationId: createReplicationInstance
      x-api-path-slug: actioncreatereplicationinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be initially allocated
          for the replication instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the replication instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the replication instance will
          be created in
        type: string
      - in: query
        name: EngineVersion
        description: The engine version number of the replication instance
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier that will be used to encrypt the content
          on the replication instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the replication instance is a Multi-AZ deployment
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the replication instance
        type: string
      - in: query
        name: ReplicationInstanceClass
        description: The compute and memory capacity of the replication instance as
          specified by the replication instance class
        type: string
      - in: query
        name: ReplicationInstanceIdentifier
        description: The replication instance identifier
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: A subnet group to associate with the replication instance
        type: string
      - in: query
        name: Tags
        description: Tags to be associated with the replication instance
        type: string
      - in: query
        name: VpcSecurityGroupIds
        description: Specifies the VPC security group to be used with the replication
          instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
  /?Action=DeleteReplicationInstance:
    get:
      summary: Delete Replication Instance
      description: Deletes the specified replication instance.
      operationId: deleteReplicationInstance
      x-api-path-slug: actiondeletereplicationinstance-get
      parameters:
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance to
          be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Instances
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