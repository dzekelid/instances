---
name: AWS RDS
x-slug: aws-rds
description: Amazon Relational Database Service (Amazon RDS) makes it easy to set
  up, operate, and scale arelational databasein the cloud. It provides cost-efficient
  and resizable capacity while managing time-consuming database administration tasks,
  freeing you up to focus on your applications and business. Amazon RDS provides you
  six familiar database engines to choose from, includingAmazon Aurora,PostgreSQL,MySQL,MariaDB,Oracle,
  andMicrosoft SQL Server.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Instances
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon RDS API Create D B Instance
  x-api-slug: amazon-rds-api
  description: Creates a new DB instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CreateDBInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actioncreatedbinstance-get-openapi.md
- name: Amazon RDS API Create D B Instance Read Replica
  x-api-slug: amazon-rds-api
  description: Creates a DB instance for a DB instance running MySQL, MariaDB, or
    PostgreSQL that acts as a Read Replica of a source DB instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=CreateDBInstanceReadReplica
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actioncreatedbinstancereadreplica-get-openapi.md
- name: Amazon RDS API Delete D B Instance
  x-api-slug: amazon-rds-api
  description: The DeleteDBInstance action deletes a previously provisioned DB instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DeleteDBInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actiondeletedbinstance-get-openapi.md
- name: Amazon RDS API Describe D B Instances
  x-api-slug: amazon-rds-api
  description: Returns information about provisioned RDS instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeDBInstances
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actiondescribedbinstances-get-openapi.md
- name: Amazon RDS API Describe Orderable D B Instance Options
  x-api-slug: amazon-rds-api
  description: Returns a list of orderable DB instance options for the specified engine.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeOrderableDBInstanceOptions
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actiondescribeorderabledbinstanceoptions-get-openapi.md
- name: Amazon RDS API Describe Reserved D B Instances
  x-api-slug: amazon-rds-api
  description: Returns information about reserved DB instances for this account, or
    about a specified reserved DB instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeReservedDBInstances
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actiondescribereserveddbinstances-get-openapi.md
- name: Amazon RDS API Describe Reserved D B Instances Offerings
  x-api-slug: amazon-rds-api
  description: Lists available reserved DB instance offerings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=DescribeReservedDBInstancesOfferings
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actiondescribereserveddbinstancesofferings-get-openapi.md
- name: Amazon RDS API Modify D B Instance
  x-api-slug: amazon-rds-api
  description: Modifies settings for a DB instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=ModifyDBInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actionmodifydbinstance-get-openapi.md
- name: Amazon RDS API Purchase Reserved D B Instances Offering
  x-api-slug: amazon-rds-api
  description: Purchases a reserved DB instance offering.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=PurchaseReservedDBInstancesOffering
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actionpurchasereserveddbinstancesoffering-get-openapi.md
- name: Amazon RDS API Reboot D B Instance
  x-api-slug: amazon-rds-api
  description: Rebooting a DB instance restarts the database engine service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=RebootDBInstance
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actionrebootdbinstance-get-openapi.md
- name: Amazon RDS API Restore D B Instance From D B Snapshot
  x-api-slug: amazon-rds-api
  description: Creates a new DB instance from a DB snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=RestoreDBInstanceFromDBSnapshot
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actionrestoredbinstancefromdbsnapshot-get-openapi.md
- name: Amazon RDS API Restore D B Instance To Point In Time
  x-api-slug: amazon-rds-api
  description: Restores a DB instance to an arbitrary point in time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: ://///?Action=RestoreDBInstanceToPointInTime
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/actionrestoredbinstancetopointintime-get-openapi.md
- name: Amazon RDS API
  x-api-slug: amazon-rds-api
  description: Amazon Relational Database Service (Amazon RDS) makes it easy to set
    up, operate, and scale arelational databasein the cloud. It provides cost-efficient
    and resizable capacity while managing time-consuming database administration tasks,
    freeing you up to focus on your applications and business. Amazon RDS provides
    you six familiar database engines to choose from, includingAmazon Aurora,PostgreSQL,MySQL,MariaDB,Oracle,
    andMicrosoft SQL Server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRDS.png
  humanURL: https://aws.amazon.com/rds/
  baseURL: :///
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-rds/openapi.md
x-common:
- type: x-articles
  url: https://aws.amazon.com/articles/Amazon-RDS
- type: x-blog
  url: https://aws.amazon.com/blogs/database/
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=291
- type: x-code
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=293
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/AmazonRDS/latest/CommandLineReference/
- type: x-customer-highlights
  url: https://aws.amazon.com/rds/customers/
- type: x-documentation
  url: http://docs.aws.amazon.com/AmazonRDS/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/rds/faqs/
- type: x-forum
  url: http://developer.amazonwebservices.com/connect/forum.jspa?forumID=60
- type: x-getting-started
  url: https://aws.amazon.com/rds/getting-started/
- type: x-partners
  url: https://aws.amazon.com/rds/partners/
- type: x-pricing
  url: https://aws.amazon.com/rds/pricing/
- type: x-service-level-agreement
  url: https://aws.amazon.com/rds/sla/
- type: x-tools
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=294
- type: x-website
  url: https://aws.amazon.com/rds/
- type: x-whats-new
  url: https://aws.amazon.com/rds/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---