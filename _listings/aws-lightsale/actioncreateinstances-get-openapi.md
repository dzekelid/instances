---
swagger: "2.0"
x-collection-name: AWS Lightsale
x-complete: 0
info:
  title: Amazon Lightsale API Create Instances
  version: 1.0.0
  description: |-
    Creates one or more Amazon Lightsail virtual private servers, or
            instances.
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