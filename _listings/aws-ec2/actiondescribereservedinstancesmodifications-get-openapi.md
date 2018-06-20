---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Describe Reserved Instances Modifications
  version: 1.0.0
  description: Describes the modifications made to your Reserved Instances.
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