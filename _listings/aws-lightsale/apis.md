---
name: AWS Lightsale
x-slug: aws-lightsale
description: Amazon Lightsail is the easiest way to get started with AWS for developers
  who just need virtual private servers. Lightsail includes everything you need to
  launch your project quickly - a virtual machine, SSD-based storage, data transfer,
  DNS management, and a static IP - for a low, predictable price. You manage those
  Lightsail servers through the Lightsail console or by using the API or command-line
  interface (CLI).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Instances
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Lightsale API Close Instance Public Ports
  x-api-slug: amazon-lightsale-api
  description: Closes the public ports on a specific Amazon Lightsail instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CloseInstancePublicPorts
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actioncloseinstancepublicports-get-openapi.md
- name: Amazon Lightsale API Create Instances
  x-api-slug: amazon-lightsale-api
  description: |-
    Creates one or more Amazon Lightsail virtual private servers, or
            instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CreateInstances
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actioncreateinstances-get-openapi.md
- name: Amazon Lightsale API Create Instances From Snapshot
  x-api-slug: amazon-lightsale-api
  description: |-
    Uses a specific snapshot as a blueprint for creating one or more new instances that are
          based on that identical configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CreateInstancesFromSnapshot
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actioncreateinstancesfromsnapshot-get-openapi.md
- name: Amazon Lightsale API Create Instance Snapshot
  x-api-slug: amazon-lightsale-api
  description: |-
    Creates a snapshot of a specific virtual private server, or
            instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=CreateInstanceSnapshot
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actioncreateinstancesnapshot-get-openapi.md
- name: Amazon Lightsale API Delete Instance
  x-api-slug: amazon-lightsale-api
  description: |-
    Deletes a specific Amazon Lightsail virtual private server, or
            instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=DeleteInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiondeleteinstance-get-openapi.md
- name: Amazon Lightsale API Delete Instance Snapshot
  x-api-slug: amazon-lightsale-api
  description: |-
    Deletes a specific snapshot of a virtual private server (or
            instance).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=DeleteInstanceSnapshot
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiondeleteinstancesnapshot-get-openapi.md
- name: Amazon Lightsale API Get Blueprints
  x-api-slug: amazon-lightsale-api
  description: Returns the list of available instance images, or blueprints.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetBlueprints
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetblueprints-get-openapi.md
- name: Amazon Lightsale API Get Instance
  x-api-slug: amazon-lightsale-api
  description: |-
    Returns information about a specific Amazon Lightsail instance, which is a virtual
          private server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstance-get-openapi.md
- name: Amazon Lightsale API Get Instance Access Details
  x-api-slug: amazon-lightsale-api
  description: |-
    Returns temporary SSH keys you can use to connect to a specific virtual private server,
          or instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstanceAccessDetails
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstanceaccessdetails-get-openapi.md
- name: Amazon Lightsale API Get Instance Metric Data
  x-api-slug: amazon-lightsale-api
  description: |-
    Returns the data points for the specified Amazon Lightsail instance metric, given an
          instance name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstanceMetricData
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstancemetricdata-get-openapi.md
- name: Amazon Lightsale API Get Instance Port States
  x-api-slug: amazon-lightsale-api
  description: |-
    Returns the port states for a specific virtual private server, or
            instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstancePortStates
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstanceportstates-get-openapi.md
- name: Amazon Lightsale API Get Instances
  x-api-slug: amazon-lightsale-api
  description: |-
    Returns information about all Amazon Lightsail virtual private servers, or
            instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstances
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstances-get-openapi.md
- name: Amazon Lightsale API Get Instance Snapshot
  x-api-slug: amazon-lightsale-api
  description: Returns information about a specific instance snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstanceSnapshot
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstancesnapshot-get-openapi.md
- name: Amazon Lightsale API Get Instance Snapshots
  x-api-slug: amazon-lightsale-api
  description: Returns all instance snapshots for the user's account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstanceSnapshots
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstancesnapshots-get-openapi.md
- name: Amazon Lightsale API Get Instance State
  x-api-slug: amazon-lightsale-api
  description: Returns the state of a specific instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=GetInstanceState
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actiongetinstancestate-get-openapi.md
- name: Amazon Lightsale API Open Instance Public Ports
  x-api-slug: amazon-lightsale-api
  description: Adds public ports to an Amazon Lightsail instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=OpenInstancePublicPorts
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actionopeninstancepublicports-get-openapi.md
- name: Amazon Lightsale API Reboot Instance
  x-api-slug: amazon-lightsale-api
  description: Restarts a specific instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=RebootInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actionrebootinstance-get-openapi.md
- name: Amazon Lightsale API Start Instance
  x-api-slug: amazon-lightsale-api
  description: Starts a specific Amazon Lightsail instance from a stopped state.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=StartInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actionstartinstance-get-openapi.md
- name: Amazon Lightsale API Stop Instance
  x-api-slug: amazon-lightsale-api
  description: Stops a specific Amazon Lightsail instance that is currently running.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: ://///?Action=StopInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/actionstopinstance-get-openapi.md
- name: Amazon Lightsale API
  x-api-slug: amazon-lightsale-api
  description: Amazon Lightsail is the easiest way to get started with AWS for developers
    who just need virtual private servers. Lightsail includes everything you need
    to launch your project quickly - a virtual machine, SSD-based storage, data transfer,
    DNS management, and a static IP - for a low, predictable price. You manage those
    Lightsail servers through the Lightsail console or by using the API or command-line
    interface (CLI).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-lightsail.png
  humanURL: https://amazonlightsail.com/
  baseURL: :///
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-lightsale/openapi.md
x-common:
- type: x-documentation
  url: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/Welcome.html?fid=6DDA37DF97F08F8B-23761D4A79F7B1E
- type: x-pricing
  url: https://amazonlightsail.com/pricing/
- type: x-website
  url: https://amazonlightsail.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---