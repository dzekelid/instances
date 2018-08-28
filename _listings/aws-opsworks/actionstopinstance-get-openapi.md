---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Stop Instance
  version: 1.0.0
  description: Stops a specified instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeInstances:
    get:
      summary: Describe Instances
      description: Requests a description of a set of instances.
      operationId: describeInstances
      x-api-path-slug: actiondescribeinstances-get
      parameters:
      - in: query
        name: InstanceIds
        description: An array of instance IDs to be described
        type: string
      - in: query
        name: LayerId
        description: A layer ID
        type: string
      - in: query
        name: StackId
        description: A stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Instances
  /?Action=DescribeRdsDbInstances:
    get:
      summary: Describe Rds Db Instances
      description: Describes Amazon RDS instances.
      operationId: describeRdsDbInstances
      x-api-path-slug: actiondescriberdsdbinstances-get
      parameters:
      - in: query
        name: RdsDbInstanceArns
        description: An array containing the ARNs of the instances to be described
        type: string
      - in: query
        name: StackId
        description: The stack ID that the instances are registered with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Rds
      - Db
      - Instances
  /?Action=AssignInstance:
    get:
      summary: Assign Instance
      description: Assign a registered instance to a layer.
      operationId: assignInstance
      x-api-path-slug: actionassigninstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: LayerIds
        description: The layer ID, which must correspond to a custom layer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assign
      - Instance
  /?Action=CreateInstance:
    get:
      summary: Create Instance
      description: Creates an instance in a specified stack.
      operationId: createInstance
      x-api-path-slug: actioncreateinstance-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: AmiId
        description: A custom AMI ID to be used to create the instance
        type: string
      - in: query
        name: Architecture
        description: The instance architecture
        type: string
      - in: query
        name: AutoScalingType
        description: For load-based or time-based instances, the type
        type: string
      - in: query
        name: AvailabilityZone
        description: The instance Availability Zone
        type: string
      - in: query
        name: BlockDeviceMappings
        description: An array of BlockDeviceMapping objects that specify the instances
          block      devices
        type: string
      - in: query
        name: EbsOptimized
        description: Whether to create an Amazon EBS-optimized instance
        type: string
      - in: query
        name: Hostname
        description: The instance host name
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: InstanceType
        description: The instance type, such as t2
        type: string
      - in: query
        name: LayerIds
        description: An array that contains the instances layer IDs
        type: string
      - in: query
        name: Os
        description: The instances operating system, which must be set to one of the
          following
        type: string
      - in: query
        name: RootDeviceType
        description: The instance root device type
        type: string
      - in: query
        name: SshKeyName
        description: The instances Amazon EC2 key-pair name
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      - in: query
        name: SubnetId
        description: The ID of the instances subnet
        type: string
      - in: query
        name: Tenancy
        description: The instances tenancy option
        type: string
      - in: query
        name: VirtualizationType
        description: The instances virtualization type, paravirtual or hvm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=DeleteInstance:
    get:
      summary: Delete Instance
      description: Deletes a specified instance, which terminates the associated Amazon
        EC2 instance.
      operationId: deleteInstance
      x-api-path-slug: actiondeleteinstance-get
      parameters:
      - in: query
        name: DeleteElasticIp
        description: Whether to delete the instance Elastic IP address
        type: string
      - in: query
        name: DeleteVolumes
        description: Whether to delete the instances Amazon EBS volumes
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=DeregisterInstance:
    get:
      summary: Deregister Instance
      description: Deregister a registered Amazon EC2 or on-premises instance.
      operationId: deregisterInstance
      x-api-path-slug: actionderegisterinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Instance
  /?Action=DeregisterRdsDbInstance:
    get:
      summary: Deregister Rds Db Instance
      description: Deregisters an Amazon RDS instance.
      operationId: deregisterRdsDbInstance
      x-api-path-slug: actionderegisterrdsdbinstance-get
      parameters:
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Rds
      - Db
      - Instance
  /?Action=RebootInstance:
    get:
      summary: Reboot Instance
      description: Reboots a specified instance.
      operationId: rebootInstance
      x-api-path-slug: actionrebootinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reboot
      - Instance
  /?Action=RegisterInstance:
    get:
      summary: Register Instance
      description: Registers instances that were created outside of AWS OpsWorks Stacks
        with a specified stack.
      operationId: registerInstance
      x-api-path-slug: actionregisterinstance-get
      parameters:
      - in: query
        name: Hostname
        description: The instances hostname
        type: string
      - in: query
        name: InstanceIdentity
        description: An InstanceIdentity object that contains the instances identity
        type: string
      - in: query
        name: PrivateIp
        description: The instances private IP address
        type: string
      - in: query
        name: PublicIp
        description: The instances public IP address
        type: string
      - in: query
        name: RsaPublicKey
        description: The instances public RSA key
        type: string
      - in: query
        name: RsaPublicKeyFingerprint
        description: The instances public RSA key fingerprint
        type: string
      - in: query
        name: StackId
        description: The ID of the stack that the instance is to be registered with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Instance
  /?Action=RegisterRdsDbInstance:
    get:
      summary: Register Rds Db Instance
      description: Registers an Amazon RDS instance with a stack.
      operationId: registerRdsDbInstance
      x-api-path-slug: actionregisterrdsdbinstance-get
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The databases master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Rds
      - Db
      - Instance
  /?Action=StartInstance:
    get:
      summary: Start Instance
      description: Starts a specified instance.
      operationId: startInstance
      x-api-path-slug: actionstartinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Instance
  /?Action=StopInstance:
    get:
      summary: Stop Instance
      description: Stops a specified instance.
      operationId: stopInstance
      x-api-path-slug: actionstopinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stop
      - Instance
  /?Action=UnassignInstance:
    get:
      summary: Unassign Instance
      description: Unassigns a registered instance from all of it's layers.
      operationId: unassignInstance
      x-api-path-slug: actionunassigninstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Unassign
      - Instance
  /?Action=UpdateInstance:
    get:
      summary: Update Instance
      description: Updates a specified instance.
      operationId: updateInstance
      x-api-path-slug: actionupdateinstance-get
      parameters:
      - in: query
        name: AgentVersion
        description: The default AWS OpsWorks Stacks agent version
        type: string
      - in: query
        name: AmiId
        description: The ID of the AMI that was used to create the instance
        type: string
      - in: query
        name: Architecture
        description: The instance architecture
        type: string
      - in: query
        name: AutoScalingType
        description: For load-based or time-based instances, the type
        type: string
      - in: query
        name: EbsOptimized
        description: This property cannot be updated
        type: string
      - in: query
        name: Hostname
        description: The instance host name
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      - in: query
        name: InstanceType
        description: The instance type, such as t2
        type: string
      - in: query
        name: LayerIds
        description: The instances layer IDs
        type: string
      - in: query
        name: Os
        description: The instances operating system, which must be set to one of the
          following
        type: string
      - in: query
        name: SshKeyName
        description: The instances Amazon EC2 key name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=UpdateRdsDbInstance:
    get:
      summary: Update Rds Db Instance
      description: Updates an Amazon RDS instance.
      operationId: updateRdsDbInstance
      x-api-path-slug: actionupdaterdsdbinstance-get
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Rds
      - Db
      - Instance
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