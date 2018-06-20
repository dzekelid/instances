---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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
---