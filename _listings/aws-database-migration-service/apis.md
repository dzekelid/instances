---
name: AWS Database Migration Service
x-slug: aws-database-migration-service
description: AWS Database Migration Service helps you migrate databases to AWS easily
  and securely. The source database remains fully operational during the migration,
  minimizing downtime to applications that rely on the database. The AWS Database
  Migration Service can migrate your data to and from most widely used commercial
  and open-source databases. The service supports homogenous migrations such as Oracle
  to Oracle, as well as heterogeneous migrations between different database platforms,
  such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It also allows
  you to stream data to Amazon Redshift from any of the supported sources including
  Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server, enabling
  consolidation and easy analysis of data in the petabyte-scale data warehouse. AWS
  Database Migration Service can also be used for continuous data replication with
  high-availability.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Instances
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Database Migration Service API Create Replication Instance
  x-api-slug: aws-database-migration-service-api
  description: Creates the replication instance using the specified parameters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=CreateReplicationInstance
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actioncreatereplicationinstance-get-openapi.md
- name: AWS Database Migration Service API Delete Replication Instance
  x-api-slug: aws-database-migration-service-api
  description: Deletes the specified replication instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DeleteReplicationInstance
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actiondeletereplicationinstance-get-openapi.md
- name: AWS Database Migration Service API Describe Orderable Replication Instances
  x-api-slug: aws-database-migration-service-api
  description: Returns information about the replication instance types that can be
    created in the specified region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DescribeOrderableReplicationInstances
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actiondescribeorderablereplicationinstances-get-openapi.md
- name: AWS Database Migration Service API Describe Replication Instances
  x-api-slug: aws-database-migration-service-api
  description: Returns information about replication instances for your account in
    the current region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DescribeReplicationInstances
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actiondescribereplicationinstances-get-openapi.md
- name: AWS Database Migration Service API Describe Replication Subnet Groups
  x-api-slug: aws-database-migration-service-api
  description: Returns information about the replication subnet groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=DescribeReplicationSubnetGroups
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actiondescribereplicationsubnetgroups-get-openapi.md
- name: AWS Database Migration Service API Modify Replication Instance
  x-api-slug: aws-database-migration-service-api
  description: Modifies the replication instance to apply new settings.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: ://///?Action=ModifyReplicationInstance
  tags: Replication Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/actionmodifyreplicationinstance-get-openapi.md
- name: AWS Database Migration Service API
  x-api-slug: aws-database-migration-service-api
  description: AWS Database Migration Service helps you migrate databases to AWS easily
    and securely. The source database remains fully operational during the migration,
    minimizing downtime to applications that rely on the database. The AWS Database
    Migration Service can migrate your data to and from most widely used commercial
    and open-source databases. The service supports homogenous migrations such as
    Oracle to Oracle, as well as heterogeneous migrations between different database
    platforms, such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It
    also allows you to stream data to Amazon Redshift from any of the supported sources
    including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE and SQL Server,
    enabling consolidation and easy analysis of data in the petabyte-scale data warehouse.
    AWS Database Migration Service can also be used for continuous data replication
    with high-availability.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AWSDatabaseMigrationService.png
  humanURL: https://aws.amazon.com/dms/
  baseURL: :///
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/aws-database-migration-service/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/dms/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/dms/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/dms/getting-started/
- type: x-partners
  url: https://aws.amazon.com/dms/partners/
- type: x-pricing
  url: https://aws.amazon.com/dms/pricing/
- type: x-schema-conversion
  url: https://aws.amazon.com/dms/#sct
- type: x-testimonials
  url: https://aws.amazon.com/dms/testimonials/
- type: x-website
  url: https://aws.amazon.com/dms/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---