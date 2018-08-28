{
  "info": {
    "name": "AWS EC2 API Describe Spot Instance Requests",
    "_postman_id": "e950a123-8304-4b6a-804f-2928f7f91934",
    "description": "Describes the Spot instance requests that belong to your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Spot Instance Requests",
      "item": [
        {
          "id": "d91842b8-71f2-4ee7-b9b6-ee86dd1e2969",
          "name": "describespotinstancerequests",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSpotInstanceRequests?AvailabilityZone=AvailabilityZone&DryRun=DryRun&EndTime=EndTime&Filter.N=Filter.N&InstanceType.N=InstanceType.N&MaxResults=MaxResults&NextToken=NextToken&ProductDescription.N=ProductDescription.N&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the Spot instance requests that belong to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "473ef074-1816-4c9c-9629-01b6119efe85"
            }
          ]
        }
      ]
    }
  ]
}