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
  /?Action=RestoreDBInstanceFromDBSnapshot&k=1:
    get:
      summary: Restore D B Instance From D B Snapshot
      description: Creates a new DB instance from a DB snapshot
      operationId: restoredbinstancefromdbsnapshot
      parameters:
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically
          to the DB instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the database instance will be
          created in
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the restored DB instance to snapshots
          of the DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the Amazon RDS DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: Name of the DB instance to create from the DB snapshot
        type: string
      - in: query
        name: DBName
        description: The database name for the restored DB instance
        type: string
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to restore from
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The DB subnet group name to use for the new instance
        type: string
      - in: query
        name: Domain
        description: Specify the Active Directory Domain to restore the instance in
        type: string
      - in: query
        name: DomainIAMRoleName
        description: Specify the name of the IAM role to be used when making API calls
          to the Directory Service
        type: string
      - in: query
        name: Engine
        description: The database engine to use for the new instance
        type: string
      - in: query
        name: Iops
        description: Specifies the amount of provisioned IOPS for the DB instance,
          expressed in I/O operations per second
        type: string
      - in: query
        name: LicenseModel
        description: License model information for the restored DB instance
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: OptionGroupName
        description: The name of the option group to be used for the restored DB instance
        type: string
      - in: query
        name: Port
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tags
        type: string
      - in: query
        name: TdeCredentialArn
        description: The ARN from the Key Store with which to associate the instance
          for TDE encryption
        type: string
      - in: query
        name: TdeCredentialPassword
        description: The password for the given ARN from the Key Store in order to
          access the device
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