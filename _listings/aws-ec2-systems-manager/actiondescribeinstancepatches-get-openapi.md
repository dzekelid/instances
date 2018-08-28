---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Describe Instance Patches
  version: 1.0.0
  description: Retrieves information about the patches on the specified instance and
    their state relative to the patch baseline being used for the instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterManagedInstance:
    get:
      summary: Deregister Managed Instance
      description: Removes the server or virtual machine from the list of registered
        servers.
      operationId: deregisterManagedInstance
      x-api-path-slug: actionderegistermanagedinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID assigned to the managed instance when you registered it
          using the activation   process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deregister
      - Managed
      - Instance
  /?Action=DescribeEffectiveInstanceAssociations:
    get:
      summary: Describe Effective Instance Associations
      description: All associations for the instance(s).
      operationId: describeEffectiveInstanceAssociations
      x-api-path-slug: actiondescribeeffectiveinstanceassociations-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance ID for which you want to view all associations
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Effective
      - Instance
      - Associations
  /?Action=DescribeInstanceAssociationsStatus:
    get:
      summary: Describe Instance Associations Status
      description: The status of the associations for the instance(s).
      operationId: describeInstanceAssociationsStatus
      x-api-path-slug: actiondescribeinstanceassociationsstatus-get
      parameters:
      - in: query
        name: InstanceId
        description: The instance IDs for which you want association status information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Associations
      - Status
  /?Action=DescribeInstanceInformation:
    get:
      summary: Describe Instance Information
      description: Describes one or more of your instances.
      operationId: describeInstanceInformation
      x-api-path-slug: actiondescribeinstanceinformation-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceInformationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Information
  /?Action=DescribeInstancePatches:
    get:
      summary: Describe Instance Patches
      description: Retrieves information about the patches on the specified instance
        and their state relative to the patch baseline being used for the instance.
      operationId: describeInstancePatches
      x-api-path-slug: actiondescribeinstancepatches-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance whose patch state information should be
          retrieved
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Patches
  /?Action=DescribeInstancePatchStates:
    get:
      summary: Describe Instance Patch States
      description: Retrieves the high-level patch state of one or more instances.
      operationId: describeInstancePatchStates
      x-api-path-slug: actiondescribeinstancepatchstates-get
      parameters:
      - in: query
        name: InstanceIds
        description: The ID of the instance whose patch state information should be
          retrieved
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of instances to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - States
  /?Action=DescribeInstancePatchStatesForPatchGroup:
    get:
      summary: Describe Instance Patch States For Patch Group
      description: Retrieves the high-level patch state for the instances in the specified
        patch group.
      operationId: describeInstancePatchStatesForPatchGroup
      x-api-path-slug: actiondescribeinstancepatchstatesforpatchgroup-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of patches to return (per page)
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group for which the patch state information
          should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
      - StatesGroup
  /?Action=UpdateManagedInstanceRole:
    get:
      summary: Update Managed Instance Role
      description: |-
        Assigns or changes an Amazon Identity and Access Management (IAM) role to the managed
           instance.
      operationId: updateManagedInstanceRole
      x-api-path-slug: actionupdatemanagedinstancerole-get
      parameters:
      - in: query
        name: IamRole
        description: The IAM role you want to assign or change
        type: string
      - in: query
        name: InstanceId
        description: The ID of the managed instance where you want to update the role
        type: string
      responses:
        200:
          description: OK
      tags:
      - Managed
      - Instance
      - Role
  /?Action=GetDeployablePatchSnapshotForInstance:
    get:
      summary: Get Deployable Patch Snapshot For Instance
      description: Retrieves the current snapshot for the patch baseline the instance
        uses.
      operationId: getDeployablePatchSnapshotForInstance
      x-api-path-slug: actiongetdeployablepatchsnapshotforinstance-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance for which the appropriate patch snapshot
          should be retrieved
        type: string
      - in: query
        name: SnapshotId
        description: The user-defined snapshot ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployable
      - SnapshotInstance
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