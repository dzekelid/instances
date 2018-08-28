---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Describe D B Instances
  version: 1.0.0
  description: Returns information about provisioned RDS instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDBInstance:
    get:
      summary: Create D B Instance
      description: Creates a new DB instance.
      operationId: createdbinstance
      x-api-path-slug: actioncreatedbinstance-get
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
      - Instances
  /?Action=CreateDBInstanceReadReplica:
    get:
      summary: Create D B Instance Read Replica
      description: Creates a DB instance for a DB instance running MySQL, MariaDB,
        or PostgreSQL that acts as a Read Replica of a source DB instance.
      operationId: createdbinstancereadreplica
      x-api-path-slug: actioncreatedbinstancereadreplica-get
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
      - Instances
  /?Action=DeleteDBInstance:
    get:
      summary: Delete D B Instance
      description: The DeleteDBInstance action deletes a previously provisioned DB
        instance.
      operationId: deletedbinstance
      x-api-path-slug: actiondeletedbinstance-get
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
      - Instances
  /?Action=DescribeDBInstances:
    get:
      summary: Describe D B Instances
      description: Returns information about provisioned RDS instances.
      operationId: describedbinstances
      x-api-path-slug: actiondescribedbinstances-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The user-supplied instance identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more DB instances to describe
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous        DescribeDBInstances
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribeOrderableDBInstanceOptions:
    get:
      summary: Describe Orderable D B Instance Options
      description: Returns a list of orderable DB instance options for the specified
        engine.
      operationId: describeorderabledbinstanceoptions
      x-api-path-slug: actiondescribeorderabledbinstanceoptions-get
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
      - Instances
  /?Action=DescribeReservedDBInstances:
    get:
      summary: Describe Reserved D B Instances
      description: Returns information about reserved DB instances for this account,
        or about a specified reserved DB instance.
      operationId: describereserveddbinstances
      x-api-path-slug: actiondescribereserveddbinstances-get
      parameters:
      - in: query
        name: DBInstanceClass
        description: The DB instance class filter value
        type: string
      - in: query
        name: Duration
        description: The duration filter value, specified in years or seconds
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
        description: The product description filter value
        type: string
      - in: query
        name: ReservedDBInstanceId
        description: The reserved DB instance identifier filter value
        type: string
      - in: query
        name: ReservedDBInstancesOfferingId
        description: The offering identifier filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DescribeReservedDBInstancesOfferings:
    get:
      summary: Describe Reserved D B Instances Offerings
      description: Lists available reserved DB instance offerings.
      operationId: describereserveddbinstancesofferings
      x-api-path-slug: actiondescribereserveddbinstancesofferings-get
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
      - Instances
  /?Action=ModifyDBInstance:
    get:
      summary: Modify D B Instance
      description: Modifies settings for a DB instance.
      operationId: modifydbinstance
      x-api-path-slug: actionmodifydbinstance-get
      parameters:
      - in: query
        name: AllocatedStorage
        description: The new storage capacity of the RDS instance
        type: string
      - in: query
        name: AllowMajorVersionUpgrade
        description: Indicates that major version upgrades are allowed
        type: string
      - in: query
        name: ApplyImmediately
        description: Specifies whether the modifications in this request and        any
          pending modifications are asynchronously applied        as soon as possible,
          regardless of the        PreferredMaintenanceWindow setting for the DB instance
        type: string
      - in: query
        name: AutoMinorVersionUpgrade
        description: Indicates that minor version upgrades will be applied automatically    to
          the DB instance during the maintenance window
        type: string
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: CACertificateIdentifier
        description: Indicates the certificate that needs to be associated with the
          instance
        type: string
      - in: query
        name: CopyTagsToSnapshot
        description: True to copy all tags from the DB instance to snapshots of the
          DB instance; otherwise false
        type: string
      - in: query
        name: DBInstanceClass
        description: The new compute and memory capacity of the DB instance
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group to apply to the DB instance
        type: string
      - in: query
        name: DBPortNumber
        description: The port number on which the database accepts connections
        type: string
      - in: query
        name: DBSecurityGroups.DBSecurityGroupName.N
        description: A list of DB security groups to authorize on this DB instance
        type: string
      - in: query
        name: DBSubnetGroupName
        description: The new DB subnet group for the DB instance
        type: string
      - in: query
        name: Domain
        description: The Active Directory Domain to move the instance to
        type: string
      - in: query
        name: DomainIAMRoleName
        description: The name of the IAM role to use when making API calls to the
          Directory Service
        type: string
      - in: query
        name: EngineVersion
        description: The version number of the database engine to upgrade to
        type: string
      - in: query
        name: Iops
        description: The new Provisioned IOPS (I/O operations per second) value for
          the RDS instance
        type: string
      - in: query
        name: LicenseModel
        description: The license model for the DB instance
        type: string
      - in: query
        name: MasterUserPassword
        description: The new password for the DB instance master user
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
        name: NewDBInstanceIdentifier
        description: The new DB instance identifier for the DB instance when renaming
          a DB            instance
        type: string
      - in: query
        name: OptionGroupName
        description: Indicates that the DB instance should be associated with the
          specified option group
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        as determined by the BackupRetentionPeriod
          parameter
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which system maintenance
          can occur, which might result in an outage
        type: string
      - in: query
        name: PromotionTier
        description: A value that specifies the order in which an Aurora Replica is
          promoted to the primary instance       after a failure of the existing primary
          instance
        type: string
      - in: query
        name: PubliclyAccessible
        description: Boolean value that indicates if the DB instance has a publicly
          resolvable DNS name
        type: string
      - in: query
        name: StorageType
        description: Specifies the storage type to be associated with the DB instance
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
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of EC2 VPC security groups to authorize on this DB instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=PurchaseReservedDBInstancesOffering:
    get:
      summary: Purchase Reserved D B Instances Offering
      description: Purchases a reserved DB instance offering.
      operationId: purchasereserveddbinstancesoffering
      x-api-path-slug: actionpurchasereserveddbinstancesoffering-get
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
      - Instances
  /?Action=RebootDBInstance:
    get:
      summary: Reboot D B Instance
      description: Rebooting a DB instance restarts the database engine service.
      operationId: rebootdbinstance
      x-api-path-slug: actionrebootdbinstance-get
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
      - Instances
  /?Action=RestoreDBInstanceFromDBSnapshot:
    get:
      summary: Restore D B Instance From D B Snapshot
      description: Creates a new DB instance from a DB snapshot.
      operationId: restoredbinstancefromdbsnapshot
      x-api-path-slug: actionrestoredbinstancefromdbsnapshot-get
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
      - Instances
  /?Action=RestoreDBInstanceToPointInTime:
    get:
      summary: Restore D B Instance To Point In Time
      description: Restores a DB instance to an arbitrary point in time.
      operationId: restoredbinstancetopointintime
      x-api-path-slug: actionrestoredbinstancetopointintime-get
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
        name: DBName
        description: The database name for the restored DB instance
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
        description: The amount of Provisioned IOPS (input/output operations per second)
          to be initially allocated for the DB instance
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
        name: RestoreTime
        description: The date and time to restore from
        type: string
      - in: query
        name: SourceDBInstanceIdentifier
        description: The identifier of the source DB instance from which to restore
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
        name: TargetDBInstanceIdentifier
        description: The name of the new database instance to be created
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
        name: UseLatestRestorableTime
        description: Specifies whether (true) or not (false) the        DB instance
          is restored from the latest backup time
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
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