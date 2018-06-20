---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Get Instance Snapshots
  version: 1.0.0
  description: Returns all instance snapshots for the user's account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CloseInstancePublicPorts:
    get:
      summary: Close Instance Public Ports
      description: Closes the public ports on a specific Amazon Lightsail instance.
      operationId: closeInstancePublicPorts
      x-api-path-slug: actioncloseinstancepublicports-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance on which youre attempting to close the
          public      ports
        type: string
      - in: query
        name: portInfo
        description: Information about the public port you are trying to close
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstances:
    get:
      summary: Create Instances
      description: |-
        Creates one or more Amazon Lightsail virtual private servers, or
                instances.
      operationId: createInstances
      x-api-path-slug: actioncreateinstances-get
      parameters:
      - in: query
        name: availabilityZone
        description: The Availability Zone in which to create your instance
        type: string
      - in: query
        name: blueprintId
        description: The ID for a virtual private server image (e
        type: string
      - in: query
        name: bundleId
        description: The bundle of specification information for your virtual private
          server (or        instance), including the pricing plan (e
        type: string
      - in: query
        name: customImageName
        description: The name for your custom image
        type: string
      - in: query
        name: instanceNames
        description: The names to use for your new Lightsail instances
        type: string
      - in: query
        name: keyPairName
        description: The name of your key pair
        type: string
      - in: query
        name: userData
        description: A launch script you can create that configures a server with
          additional user data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstancesFromSnapshot:
    get:
      summary: Create Instances From Snapshot
      description: |-
        Uses a specific snapshot as a blueprint for creating one or more new instances that are
              based on that identical configuration.
      operationId: createInstancesFromSnapshot
      x-api-path-slug: actioncreateinstancesfromsnapshot-get
      parameters:
      - in: query
        name: availabilityZone
        description: The Availability Zone where you want to create your instances
        type: string
      - in: query
        name: bundleId
        description: The bundle of specification information for your virtual private
          server (or        instance), including the pricing plan (e
        type: string
      - in: query
        name: instanceNames
        description: The names for your new instances
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name of the instance snapshot on which you are basing your
          new instances
        type: string
      - in: query
        name: keyPairName
        description: The name for your key pair
        type: string
      - in: query
        name: userData
        description: You can create a launch script that configures a server with
          additional user data
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=CreateInstanceSnapshot:
    get:
      summary: Create Instance Snapshot
      description: |-
        Creates a snapshot of a specific virtual private server, or
                instance.
      operationId: createInstanceSnapshot
      x-api-path-slug: actioncreateinstancesnapshot-get
      parameters:
      - in: query
        name: instanceName
        description: The Lightsail instance on which to base your snapshot
        type: string
      - in: query
        name: instanceSnapshotName
        description: The name for your new snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteInstance:
    get:
      summary: Delete Instance
      description: |-
        Deletes a specific Amazon Lightsail virtual private server, or
                instance.
      operationId: deleteInstance
      x-api-path-slug: actiondeleteinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=DeleteInstanceSnapshot:
    get:
      summary: Delete Instance Snapshot
      description: |-
        Deletes a specific snapshot of a virtual private server (or
                instance).
      operationId: deleteInstanceSnapshot
      x-api-path-slug: actiondeleteinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetBlueprints:
    get:
      summary: Get Blueprints
      description: Returns the list of available instance images, or blueprints.
      operationId: getBlueprints
      x-api-path-slug: actiongetblueprints-get
      parameters:
      - in: query
        name: includeInactive
        description: A Boolean value indicating whether to include inactive results
          in your      request
        type: string
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get blueprints      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstance:
    get:
      summary: Get Instance
      description: |-
        Returns information about a specific Amazon Lightsail instance, which is a virtual
              private server.
      operationId: getInstance
      x-api-path-slug: actiongetinstance-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceAccessDetails:
    get:
      summary: Get Instance Access Details
      description: |-
        Returns temporary SSH keys you can use to connect to a specific virtual private server,
              or instance.
      operationId: getInstanceAccessDetails
      x-api-path-slug: actiongetinstanceaccessdetails-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance to access
        type: string
      - in: query
        name: protocol
        description: The protocol to use to connect to your instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceMetricData:
    get:
      summary: Get Instance Metric Data
      description: |-
        Returns the data points for the specified Amazon Lightsail instance metric, given an
              instance name.
      operationId: getInstanceMetricData
      x-api-path-slug: actiongetinstancemetricdata-get
      parameters:
      - in: query
        name: endTime
        description: The end time of the time period
        type: string
      - in: query
        name: instanceName
        description: The name of the instance for which you want to get metrics data
        type: string
      - in: query
        name: metricName
        description: The metric name to get data about
        type: string
      - in: query
        name: period
        description: The time period for which you are requesting data
        type: string
      - in: query
        name: startTime
        description: The start time of the time period
        type: string
      - in: query
        name: statistics
        description: The instance statistics
        type: string
      - in: query
        name: unit
        description: The unit
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstancePortStates:
    get:
      summary: Get Instance Port States
      description: |-
        Returns the port states for a specific virtual private server, or
                instance.
      operationId: getInstancePortStates
      x-api-path-slug: actiongetinstanceportstates-get
      parameters:
      - in: query
        name: instanceName
        description: The name of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstances:
    get:
      summary: Get Instances
      description: |-
        Returns information about all Amazon Lightsail virtual private servers, or
                instances.
      operationId: getInstances
      x-api-path-slug: actiongetinstances-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instances      request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshot:
    get:
      summary: Get Instance Snapshot
      description: Returns information about a specific instance snapshot.
      operationId: getInstanceSnapshot
      x-api-path-slug: actiongetinstancesnapshot-get
      parameters:
      - in: query
        name: instanceSnapshotName
        description: The name of the snapshot for which you are requesting information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
  /?Action=GetInstanceSnapshots:
    get:
      summary: Get Instance Snapshots
      description: Returns all instance snapshots for the user's account.
      operationId: getInstanceSnapshots
      x-api-path-slug: actiongetinstancesnapshots-get
      parameters:
      - in: query
        name: pageToken
        description: A token used for advancing to the next page of results from your
          get instance snapshots      request
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