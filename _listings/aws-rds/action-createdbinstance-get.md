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
  /?Action=CreateDBInstance&k=1:
    get:
      summary: Create D B Instance
      description: Creates a new DB instance
      operationId: createdbinstance
      parameters:
      - in: query
        name: AllocatedStorage
        description: The amount of storage (in gigabytes) to be initially allocated
          for the database instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor engine upgrades will be applied automatically
          to the DB instance during the maintenance window
        type: string
      - in: query
        name: AvailabilityZone
        description: The EC2 Availability Zone that the database instance will be
          created in
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days for which automated backups are retained
        type: string
      - in: query
        name: CharacterSetName
        description: For supported engines, indicates that the DB instance should
          be associated with the specified CharacterSet
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the DB instance to snapshots of the
          DB instance; otherwise false
        type: string
      - in: query
        name: DBClusterIdentifier
        description: The identifier of the DB cluster that the instance will belong
          to
        type: string
      - in: query
        name: DBInstanceClass
        description: The compute and memory capacity of the DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBName
        description: The meaning of this parameter differs according to the database
          engine you use
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group to associate with this DB
          instance
        type: string
      - in: query
        name: DBSecurityGroups.DBSecurityGroupName.N
        description: A list of DB security groups to associate with this DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: A DB subnet group to associate with this DB instance
        type: string
      - in: query
        name: Domain
        description: Specify the Active Directory Domain to create the instance in
        type: string
      - in: query
        name: DomainIAMRoleName
        description: Specify the name of the IAM role to be used when making API calls
          to the Directory Service
        type: string
      - in: query
        name: Engine
        description: The name of the database engine to be used for this instance
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to use
        type: string
      - in: query
        name: Iops
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
        type: string
      - in: query
        name: KmsKeyId
        description: The KMS key identifier for an encrypted DB instance
        type: string
      - in: query
        name: LicenseModel
        description: License model information for this DB instance
        type: string
      - in: query
        name: MasterUsername
        description: The name of master user for the client DB instance
        type: string
      - in: query
        name: MasterUserPassword
        description: The password for the master database user
        type: string
      - in: query
        name: MonitoringInterval
        description: The interval, in seconds, between points when Enhanced Monitoring
          metrics are collected for the DB instance
        type: string
      - in: query
        name: MonitoringRoleArn
        description: The ARN for the IAM role that permits RDS to send enhanced monitoring
          metrics to CloudWatch Logs
        type: string
      - in: query
        name: MultiAZ
        description: Specifies if the DB instance is a Multi-AZ deployment
        type: string
      - in: query
        name: OptionGroupName
        description: Indicates that the DB instance should be associated with the
          specified option group
        type: string
      - in: query
        name: Port
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        using the BackupRetentionPeriod parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range during which system maintenance can occur,
          in Universal Coordinated Time (UTC)
        type: string
      - in: query
        name: PromotionTier
        description: A value that specifies the order in which an Aurora Replica is
          promoted to the primary instance       after a failure of the existing primary
          instance
        type: string
      - in: query
        name: PubliclyAccessible
        description: Specifies the accessibility options for the DB instance
        type: string
      - in: query
        name: StorageEncrypted
        description: Specifies whether the DB instance is encrypted
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
      - in: query
        name: Timezone
        description: The time zone of the DB instance
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to associate with this DB instance
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