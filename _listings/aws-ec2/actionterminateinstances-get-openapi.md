---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Terminate Instances
  version: 1.0.0
  description: Shuts down one or more instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RunInstances:
    get:
      summary: Run Instances
      description: |-
        Launches the specified number of instances using an AMI for which you have
                    permissions.
      operationId: runinstances
      x-api-path-slug: actionruninstances-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances
  /?Action=StartInstances:
    get:
      summary: Start Instances
      description: Starts an Amazon EBS-backed AMI that you've previously stopped.
      operationId: startinstances
      x-api-path-slug: actionstartinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Force
        description: Forces the instances to stop
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances
  /?Action=StopInstances:
    get:
      summary: Stop Instances
      description: Stops an Amazon EBS-backed instance.
      operationId: stopinstances
      x-api-path-slug: actionstopinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instances
  /?Action=TerminateInstances:
    get:
      summary: Terminate Instances
      description: Shuts down one or more instances.
      operationId: terminateinstances
      x-api-path-slug: actionterminateinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Terminal Instances
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