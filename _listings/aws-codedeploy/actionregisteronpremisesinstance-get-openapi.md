---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Register On Premises Instance
  version: 1.0.0
  description: Registers an on-premises instance.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddTagsToOnPremisesInstances:
    get:
      summary: Add Tags To On Premises Instances
      description: Adds tags to on-premises instances.
      operationId: addTagsToOnPremisesInstances
      x-api-path-slug: actionaddtagstoonpremisesinstances-get
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances to which to add tags
        type: string
      - in: query
        name: tags
        description: The tag key-value pairs to add to the on-premises instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Premises Instances Tags
  /?Action=BatchGetDeploymentInstances:
    get:
      summary: Batch Get Deployment Instances
      description: |-
        Gets information about one or more instance that are part of a deployment
                    group.
      operationId: batchGetDeploymentInstances
      x-api-path-slug: actionbatchgetdeploymentinstances-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceIds
        description: The unique IDs of instances in the deployment group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=BatchGetOnPremisesInstances:
    get:
      summary: Batch Get On Premises Instances
      description: Gets information about one or more on-premises instances.
      operationId: batchGetOnPremisesInstances
      x-api-path-slug: actionbatchgetonpremisesinstances-get
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances about which to get information
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
  /?Action=ListDeploymentInstances:
    get:
      summary: List Deployment Instances
      description: |-
        Lists the instance for a deployment associated with the applicable IAM user or AWS
                    account.
      operationId: listDeploymentInstances
      x-api-path-slug: actionlistdeploymentinstances-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceStatusFilter
        description: 'A subset of instances to list by status:'
        type: string
      - in: query
        name: nextToken
        description: An identifier returned from the previous list deployment instances
          call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=ListOnPremisesInstances:
    get:
      summary: List On Premises Instances
      description: Gets a list of names for one or more on-premises instances.
      operationId: listOnPremisesInstances
      x-api-path-slug: actionlistonpremisesinstances-get
      parameters:
      - in: query
        name: nextToken
        description: An identifier returned from the previous list on-premises instances
          call
        type: string
      - in: query
        name: registrationStatus
        description: 'The registration status of the on-premises instances:'
        type: string
      - in: query
        name: tagFilters
        description: The on-premises instance tags that will be used to restrict the
          corresponding            on-premises instance names returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
  /?Action=RemoveTagsFromOnPremisesInstances:
    get:
      summary: Remove Tags From On Premises Instances
      description: Removes one or more tags from one or more on-premises instances.
      operationId: removeTagsFromOnPremisesInstances
      x-api-path-slug: actionremovetagsfromonpremisesinstances-get
      parameters:
      - in: query
        name: instanceNames
        description: The names of the on-premises instances from which to remove tags
        type: string
      - in: query
        name: tags
        description: The tag key-value pairs to remove from the on-premises instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
  /?Action=DeregisterOnPremisesInstance:
    get:
      summary: Deregister On Premises Instance
      description: Deregisters an on-premises instance.
      operationId: deregisterOnPremisesInstance
      x-api-path-slug: actionderegisteronpremisesinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the on-premises instance to deregister
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
  /?Action=GetDeploymentInstance:
    get:
      summary: Get Deployment Instance
      description: Gets information about an instance as part of a deployment.
      operationId: getDeploymentInstance
      x-api-path-slug: actiongetdeploymentinstance-get
      parameters:
      - in: query
        name: deploymentId
        description: The unique ID of a deployment
        type: string
      - in: query
        name: instanceId
        description: The unique ID of an instance in the deployment group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Instances
  /?Action=GetOnPremisesInstance:
    get:
      summary: Get On Premises Instance
      description: Gets information about an on-premises instance.
      operationId: getOnPremisesInstance
      x-api-path-slug: actiongetonpremisesinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the on-premises instance about which to get information
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
  /?Action=RegisterOnPremisesInstance:
    get:
      summary: Register On Premises Instance
      description: Registers an on-premises instance.
      operationId: registerOnPremisesInstance
      x-api-path-slug: actionregisteronpremisesinstance-get
      parameters:
      - in: query
        name: iamSessionArn
        description: The ARN of the IAM session to associate with the on-premises
          instance
        type: string
      - in: query
        name: iamUserArn
        description: The ARN of the IAM user to associate with the on-premises instance
        type: string
      - in: query
        name: instanceName
        description: The name of the on-premises instance to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
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