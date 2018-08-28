---
swagger: "2.0"
x-collection-name: AWS CloudHSM
x-complete: 1
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateHsm:
    get:
      summary: Create HSM
      description: Creates an uninitialized HSM instance.
      operationId: createHsm
      x-api-path-slug: actioncreatehsm-get
      parameters:
      - in: query
        name: ClientToken
        description: A user-defined token to ensure idempotence
        type: string
      - in: query
        name: EniIp
        description: The IP address to assign to the HSMs ENI
        type: string
      - in: query
        name: ExternalId
        description: The external ID from IamRoleArn, if present
        type: string
      - in: query
        name: IamRoleArn
        description: The ARN of an IAM role to enable the AWS CloudHSM service to
          allocate an ENI on your      behalf
        type: string
      - in: query
        name: SshKey
        description: The SSH public key to install on the HSM
        type: string
      - in: query
        name: SubnetId
        description: The identifier of the subnet in your VPC in which to place the
          HSM
        type: string
      - in: query
        name: SubscriptionType
        description: Specifies the type of subscription for the HSM
        type: string
      - in: query
        name: SyslogIp
        description: The IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=DeleteHsm:
    get:
      summary: Delete HSM
      description: Deletes an HSM.
      operationId: deleteHsm
      x-api-path-slug: actiondeletehsm-get
      parameters:
      - in: query
        name: HsmArn
        description: The ARN of the HSM to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=DescribeHsm:
    get:
      summary: Describe HSM
      description: Retrieves information about an HSM.
      operationId: describeHsm
      x-api-path-slug: actiondescribehsm-get
      parameters:
      - in: query
        name: HsmArn
        description: The ARN of the HSM
        type: string
      - in: query
        name: HsmSerialNumber
        description: The serial number of the HSM
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=ListHsms:
    get:
      summary: List HSM
      description: |-
        Retrieves the identifiers of all of the HSMs provisioned for the current
              customer.
      operationId: listHsms
      x-api-path-slug: actionlisthsms-get
      parameters:
      - in: query
        name: NextToken
        description: The NextToken value from a previous call to ListHsms
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
  /?Action=ModifyHsm:
    get:
      summary: Modify HSM
      description: Modifies an HSM.
      operationId: modifyHsm
      x-api-path-slug: actionmodifyhsm-get
      parameters:
      - in: query
        name: EniIp
        description: The new IP address for the elastic network interface (ENI) attached
          to the      HSM
        type: string
      - in: query
        name: ExternalId
        description: The new external ID
        type: string
      - in: query
        name: HsmArn
        description: The ARN of the HSM to modify
        type: string
      - in: query
        name: IamRoleArn
        description: The new IAM role ARN
        type: string
      - in: query
        name: SubnetId
        description: The new identifier of the subnet that the HSM is in
        type: string
      - in: query
        name: SyslogIp
        description: The new IP address for the syslog monitoring server
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Instances
---