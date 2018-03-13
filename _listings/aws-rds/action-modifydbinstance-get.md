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
  /?Action=ModifyDBInstance&k=1:
    get:
      summary: Modify D B Instance
      description: Modifies settings for a DB instance
      operationId: modifydbinstance
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