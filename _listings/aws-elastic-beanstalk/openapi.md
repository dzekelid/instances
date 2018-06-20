---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeInstancesHealth:
    get:
      summary: Describe Instances Health
      description: |-
        Retrives detailed information about the health of instances in your AWS Elastic
              Beanstalk.
      operationId: describeInstancesHealth
      x-api-path-slug: actiondescribeinstanceshealth-get
      parameters:
      - in: query
        name: AttributeNames.member.N
        description: Specifies the response elements you wish to receive
        type: string
      - in: query
        name: EnvironmentId
        description: Specify the AWS Elastic Beanstalk environment by ID
        type: string
      - in: query
        name: EnvironmentName
        description: Specify the AWS Elastic Beanstalk environment by name
        type: string
      - in: query
        name: NextToken
        description: Specify the pagination token returned by a previous call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances Health
---