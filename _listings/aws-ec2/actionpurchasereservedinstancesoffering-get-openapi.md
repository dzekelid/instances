---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Purchase Reserved Instances Offering
  version: 1.0.0
  description: Purchases a Reserved Instance for use with your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptReservedInstancesExchangeQuote:
    get:
      summary: Accept Reserved Instances Exchange Quote
      description: Accepts the Convertible Reserved Instance exchange quote described
        in the GetReservedInstancesExchangeQuote call.
      operationId: acceptreservedinstancesexchangequote
      x-api-path-slug: actionacceptreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ReservedInstancesListingId
        description: The ID of the Reserved Instance listing
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=CancelReservedInstancesListing:
    get:
      summary: Cancel Reserved Instances Listing
      description: Cancels the specified Reserved Instance listing in the Reserved
        Instance Marketplace.
      operationId: cancelreservedinstanceslisting
      x-api-path-slug: actioncancelreservedinstanceslisting-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of yourlistings
        type: string
      - in: query
        name: InstanceCount
        description: The number of instances that are a part of a Reserved Instance
          account to be listed in the Reserved Instance Marketplace
        type: string
      - in: query
        name: PriceSchedules.N
        description: A list specifying the price of the Standard Reserved Instance
          for each month remaining in the Reserved Instance term
        type: string
      - in: query
        name: ReservedInstancesId
        description: The ID of the active Standard Reserved Instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=CreateReservedInstancesListing:
    get:
      summary: Create Reserved Instances Listing
      description: "Creates a listing for Amazon EC2 Standard Reserved Instances to
        be sold in the Reserved Instance\n\t\t\tMarketplace."
      operationId: createreservedinstanceslisting
      x-api-path-slug: actioncreatereservedinstanceslisting-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: OfferingClass
        description: Describes whether the Reserved Instance is Standard or Convertible
        type: string
      - in: query
        name: OfferingType
        description: The Reserved Instance offering type
        type: string
      - in: query
        name: ReservedInstancesId.N
        description: One or more Reserved Instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=DescribeClassicLinkInstances:
    get:
      summary: Describe Classic Link Instances
      description: Describes one or more of your linked EC2-Classic instances.
      operationId: describeclassiclinkinstances
      x-api-path-slug: actiondescribeclassiclinkinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: VpcId.N
        description: One or more VPCs for which you want to describe the ClassicLink
          status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=DescribeInstances:
    get:
      summary: Describe Instances
      description: Describes one or more of your instances.
      operationId: describeinstances
      x-api-path-slug: actiondescribeinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: IncludeAllInstances
        description: When true, includes the health status for all instances
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=DescribeReservedInstances:
    get:
      summary: Describe Reserved Instances
      description: Describes one or more of the Reserved Instances that you purchased.
      operationId: describereservedinstances
      x-api-path-slug: actiondescribereservedinstances-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: ReservedInstancesId
        description: One or more Reserved Instance IDs
        type: string
      - in: query
        name: ReservedInstancesListingId
        description: One or more Reserved Instance listing IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=DescribeReservedInstancesListings:
    get:
      summary: Describe Reserved Instances Listings
      description: Describes your account's Reserved Instance listings in the Reserved
        Instance Marketplace.
      operationId: describereservedinstanceslistings
      x-api-path-slug: actiondescribereservedinstanceslistings-get
      parameters:
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      - in: query
        name: ReservedInstancesModificationId.N
        description: IDs for the submitted modification request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=DescribeReservedInstancesModifications:
    get:
      summary: Describe Reserved Instances Modifications
      description: Describes the modifications made to your Reserved Instances.
      operationId: describereservedinstancesmodifications
      x-api-path-slug: actiondescribereservedinstancesmodifications-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: The Availability Zone in which the Reserved Instance can be used
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: IncludeMarketplace
        description: Include Reserved Instance Marketplace offerings in the response
        type: string
      - in: query
        name: InstanceTenancy
        description: The tenancy of the instances covered by the reservation
        type: string
      - in: query
        name: InstanceType
        description: The instance type that the reservation will cover (for example,
          m1
        type: string
      - in: query
        name: MaxDuration
        description: The maximum duration (in seconds) to filter when searching for
          offerings
        type: string
      - in: query
        name: MaxInstanceCount
        description: The maximum number of instances to filter when searching for
          offerings
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: MinDuration
        description: The minimum duration (in seconds) to filter when searching for
          offerings
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      - in: query
        name: OfferingClass
        description: The offering class of the Reserved Instance
        type: string
      - in: query
        name: OfferingType
        description: The Reserved Instance offering type
        type: string
      - in: query
        name: ProductDescription
        description: The Reserved Instance product platform description
        type: string
      - in: query
        name: ReservedInstancesOfferingId.N
        description: One or more Reserved Instances offering IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=DescribeReservedInstancesOfferings:
    get:
      summary: Describe Reserved Instances Offerings
      description: Describes Reserved Instance offerings that are available for purchase.
      operationId: describereservedinstancesofferings
      x-api-path-slug: actiondescribereservedinstancesofferings-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: ReservedInstanceId.N
        description: The IDs of the Convertible Reserved Instances to exchange
        type: string
      - in: query
        name: TargetConfiguration.N
        description: The configuration requirements of the Convertible Reserved Instances
          to exchange for your current      Convertible Reserved Instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=DescribeScheduledInstances:
    get:
      summary: Describe Scheduled Instances
      description: Describes one or more of your Scheduled Instances.
      operationId: describescheduledinstances
      x-api-path-slug: actiondescribescheduledinstances-get
      responses:
        200:
          description: OK
      tags:
      - Scheduled Server Instances
  /?Action=DescribeSpotFleetInstances:
    get:
      summary: Describe Spot Fleet Instances
      description: Describes the running instances for the specified Spot fleet.
      operationId: describespotfleetinstances
      x-api-path-slug: actiondescribespotfleetinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: EventType
        description: The type of events to describe
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of results
        type: string
      - in: query
        name: SpotFleetRequestId
        description: The ID of the Spot fleet request
        type: string
      - in: query
        name: StartTime
        description: The starting date and time for the events, in UTC format (for
          example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Fleet Instance
  /?Action=GetReservedInstancesExchangeQuote:
    get:
      summary: Get Reserved Instances Exchange Quote
      description: Returns details about the values and term of your specified Convertible
        Reserved Instances.
      operationId: getreservedinstancesexchangequote
      x-api-path-slug: actiongetreservedinstancesexchangequote-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique, case-sensitive token you provide to ensure idempotency
          of your modification request
        type: string
      - in: query
        name: ReservedInstancesConfigurationSetItemType.N
        description: The configuration settings for the Reserved Instances to modify
        type: string
      - in: query
        name: ReservedInstancesId.N
        description: The IDs of the Reserved Instances to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instances
  /?Action=ModifyReservedInstances:
    get:
      summary: Modify Reserved Instances
      description: Modifies the Availability Zone, instance count, instance type,
        or network platform (EC2-Classic or EC2-VPC) of your Standard Reserved Instances.
      operationId: modifyreservedinstances
      x-api-path-slug: actionmodifyreservedinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceCount
        description: The number of Reserved Instances to purchase
        type: string
      - in: query
        name: LimitPrice
        description: Specified for Reserved Instance Marketplace offerings to limit
          the total order and ensure that the Reserved Instances are not purchased
          at unexpected prices
        type: string
      - in: query
        name: ReservedInstancesOfferingId
        description: The ID of the Reserved Instance offering to purchase
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=MonitorInstances:
    get:
      summary: Monitor Instances
      description: Enables detailed monitoring for a running instance.
      operationId: monitorinstances
      x-api-path-slug: actionmonitorinstances-get
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
      - Monitor Instance
  /?Action=PurchaseReservedInstancesOffering:
    get:
      summary: Purchase Reserved Instances Offering
      description: Purchases a Reserved Instance for use with your account.
      operationId: purchasereservedinstancesoffering
      x-api-path-slug: actionpurchasereservedinstancesoffering-get
      parameters:
      - in: query
        name: PrincipalArn
        description: The ARN of the principal, which can be an IAM role, IAM user,
          or the root user
        type: string
      - in: query
        name: Resource
        description: 'The type of resource: instance | reservation |        snapshot
          | volume'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Instance
  /?Action=PurchaseScheduledInstances:
    get:
      summary: Purchase Scheduled Instances
      description: Purchases one or more Scheduled Instances with the specified schedule.
      operationId: purchasescheduledinstances
      x-api-path-slug: actionpurchasescheduledinstances-get
      responses:
        200:
          description: OK
      tags:
      - Scheduled Instance
  /?Action=RebootInstances:
    get:
      summary: Reboot Instances
      description: Requests a reboot of one or more instances.
      operationId: rebootinstances
      x-api-path-slug: actionrebootinstances-get
      parameters:
      - in: query
        name: Description
        description: Descriptive text about the health state of your instance
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: EndTime
        description: The time at which the reported instance health state ended
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instances
        type: string
      - in: query
        name: ReasonCode.N
        description: One or more reason codes that describes the health state of your
          instance
        type: string
      - in: query
        name: StartTime
        description: The time at which the reported instance health state began
        type: string
      - in: query
        name: Status
        description: The status of all instances listed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=RequestSpotInstances:
    get:
      summary: Request Spot Instances
      description: Creates a Spot instance request.
      operationId: requestspotinstances
      x-api-path-slug: actionrequestspotinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: SpotFleetRequestId.N
        description: The IDs of the Spot fleet requests
        type: string
      - in: query
        name: TerminateInstances
        description: Indicates whether to terminate instances for a Spot fleet request
          if it is canceled successfully
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Instance
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
  /?Action=RunScheduledInstances:
    get:
      summary: Run Scheduled Instances
      description: Launches the specified Scheduled Instances.
      operationId: runscheduledinstances
      x-api-path-slug: actionrunscheduledinstances-get
      parameters:
      - in: query
        name: CidrIp
        description: The CIDR IPv4 address range
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: FromPort
        description: The start of port range for the TCP and UDP protocols, or an
          ICMP type number
        type: string
      - in: query
        name: GroupId
        description: The ID of the security group
        type: string
      - in: query
        name: IpPermissions.N
        description: A set of IP permissions
        type: string
      - in: query
        name: IpProtocol
        description: The IP protocol name or number
        type: string
      - in: query
        name: SourceSecurityGroupName
        description: The name of a destination security group
        type: string
      - in: query
        name: SourceSecurityGroupOwnerId
        description: The AWS account number for a destination security group
        type: string
      - in: query
        name: ToPort
        description: The end of port range for the TCP and UDP protocols, or an ICMP
          type number
        type: string
      responses:
        200:
          description: OK
      tags:
      - Scheduled Instances
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
  /?Action=UnmonitorInstances:
    get:
      summary: Unmonitor Instances
      description: Disables detailed monitoring for a running instance.
      operationId: unmonitorinstances
      x-api-path-slug: actionunmonitorinstances-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InternetGatewayId
        description: The ID of the Internet gateway
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ImportInstance:
    get:
      summary: Import Instance
      description: Creates an import instance task using metadata from the specified
        disk image.
      operationId: importinstance
      x-api-path-slug: actionimportinstance-get
      responses:
        200:
          description: OK
      tags:
      - Instance
  /?Action=BundleInstance:
    get:
      summary: Bundle Instance
      description: Bundles an Amazon instance store-backed Windows instance.
      operationId: bundleinstance
      x-api-path-slug: actionbundleinstance-get
      parameters:
      - in: query
        name: BundleId
        description: The ID of the bundle task
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Bundle Instance
  /?Action=CancelSpotInstanceRequests:
    get:
      summary: Cancel Spot Instance Requests
      description: Cancels one or more Spot instance requests.
      operationId: cancelspotinstancerequests
      x-api-path-slug: actioncancelspotinstancerequests-get
      parameters:
      - in: query
        name: Bucket
        description: The Amazon S3 bucket in which to store the Spot instance data
          feed
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Prefix
        description: A prefix for the data feed file names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Instance
  /?Action=ConfirmProductInstance:
    get:
      summary: Confirm Product Instance
      description: Determines whether a product code is associated with an instance.
      operationId: confirmproductinstance
      x-api-path-slug: actionconfirmproductinstance-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to bundle
        type: string
      - in: query
        name: Storage
        description: The bucket in which to store the AMI
        type: string
      responses:
        200:
          description: OK
      tags:
      - Product Instance
  /?Action=CreateInstanceExportTask:
    get:
      summary: Create Instance Export Task
      description: Exports a running or stopped instance to an S3 bucket.
      operationId: createinstanceexporttask
      x-api-path-slug: actioncreateinstanceexporttask-get
      parameters:
      - in: query
        name: ExportTaskId.N
        description: One or more export task IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Export Task
  /?Action=DescribeInstanceAttribute:
    get:
      summary: Describe Instance Attribute
      description: Describes the specified attribute of the specified instance.
      operationId: describeinstanceattribute
      x-api-path-slug: actiondescribeinstanceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token to request the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=DescribeInstanceStatus:
    get:
      summary: Describe Instance Status
      description: Describes the status of one or more instances.
      operationId: describeinstancestatus
      x-api-path-slug: actiondescribeinstancestatus-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance Status
  /?Action=DescribeScheduledInstanceAvailability:
    get:
      summary: Describe Scheduled Instance Availability
      description: Finds available schedules that meet the specified criteria.
      operationId: describescheduledinstanceavailability
      x-api-path-slug: actiondescribescheduledinstanceavailability-get
      responses:
        200:
          description: OK
      tags:
      - Server Instance Availability
  /?Action=DescribeSpotInstanceRequests:
    get:
      summary: Describe Spot Instance Requests
      description: Describes the Spot instance requests that belong to your account.
      operationId: describespotinstancerequests
      x-api-path-slug: actiondescribespotinstancerequests-get
      parameters:
      - in: query
        name: AvailabilityZone
        description: Filters the results by the specified Availability Zone
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EndTime
        description: The date and time, up to the current date, from which to stop
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InstanceType.N
        description: Filters the results by the specified instance types
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of results
        type: string
      - in: query
        name: ProductDescription.N
        description: Filters the results by the specified basic product descriptions
        type: string
      - in: query
        name: StartTime
        description: The date and time, up to the past 90 days, from which to start
          retrieving the price history data,        in UTC format (for example, YYYY-MM-DDTHH:MM:SSZ)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Spot Instance Requests
  /?Action=ModifyInstanceAttribute:
    get:
      summary: Modify Instance Attribute
      description: Modifies the specified attribute of the specified instance.
      operationId: modifyinstanceattribute
      x-api-path-slug: actionmodifyinstanceattribute-get
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
      - Server Instance
  /?Action=ModifyInstancePlacement:
    get:
      summary: Modify Instance Placement
      description: |-
        Set the instance affinity value for a specific stopped instance and modify the
                    instance tenancy setting.
      operationId: modifyinstanceplacement
      x-api-path-slug: actionmodifyinstanceplacement-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of the request
        type: string
      - in: query
        name: CurrencyCode
        description: The currency in which the totalUpfrontPrice, LimitPrice,            and
          totalHourlyPrice amounts are specified
        type: string
      - in: query
        name: HostIdSet.N
        description: The ID/s of the Dedicated Host/s that the reservation will be
          associated            with
        type: string
      - in: query
        name: LimitPrice
        description: The specified limit is checked against the total upfront cost
          of the reservation            (calculated as the offerings upfront cost
          multiplied by the host count)
        type: string
      - in: query
        name: OfferingId
        description: The ID of the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
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