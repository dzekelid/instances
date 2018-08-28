swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AttachInstances:
    get:
      summary: Attach Instances
      description: Attaches one or more EC2 instances to the specified Auto Scaling
        group.
      operationId: attachInstances
      x-api-path-slug: actionattachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=DescribeAutoScalingInstances:
    get:
      summary: Describe Auto Scaling Instances
      description: Describes one or more Auto Scaling instances.
      operationId: describeAutoScalingInstances
      x-api-path-slug: actiondescribeautoscalinginstances-get
      parameters:
      - in: query
        name: InstanceIds.member.N
        description: The instances to describe; up to 50 instance IDs
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Auto Scaling Instances
  /?Action=DetachInstances:
    get:
      summary: Detach Instances
      description: Removes one or more instances from the specified Auto Scaling group.
      operationId: detachInstances
      x-api-path-slug: actiondetachinstances-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If True, the Auto Scaling group decrements the desired capacity
          value by the number of instances detached
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances
  /?Action=SetInstanceHealth:
    get:
      summary: Set Instance Health
      description: Sets the health status of the specified instance.
      operationId: setInstanceHealth
      x-api-path-slug: actionsetinstancehealth-get
      parameters:
      - in: query
        name: HealthStatus
        description: The health status of the instance
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldRespectGracePeriod
        description: If the Auto Scaling group of the specified instance has a HealthCheckGracePeriod             specified
          for the group, by default, this call will respect the grace period
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Health
  /?Action=SetInstanceProtection:
    get:
      summary: Set Instance Protection
      description: Updates the instance protection settings of the specified instances.
      operationId: setInstanceProtection
      x-api-path-slug: actionsetinstanceprotection-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instance IDs
        type: string
      - in: query
        name: ProtectedFromScaleIn
        description: Indicates whether the instance is protected from termination
          by Auto Scaling when scaling in
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Protection
  /?Action=TerminateInstanceInAutoScalingGroup:
    get:
      summary: Terminate Instance In Auto Scaling Group
      description: Terminates the specified instance and optionally adjusts the desired
        group size.
      operationId: terminateInstanceInAutoScalingGroup
      x-api-path-slug: actionterminateinstanceinautoscalinggroup-get
      parameters:
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: If true, terminating the instance also decrements the size of
          the Auto Scaling group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Auto Scaling