---
name: Google Cloud SQL
description: Cloud SQL is a fully-managed database service that makes it easy to set
  up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL databases
  in the cloud. Cloud SQL offers high performance, scalability, and convenience. Hosted
  on Google Cloud Platform, Cloud SQL provides a database infrastructure for applications
  running anywhere.
image: ""
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Google APIs
- Database
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Cloud SQL API
  description: Cloud SQL is a fully-managed database service that makes it easy to
    set up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL
    databases in the cloud
  image: ""
  humanURL: ""
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projects-project-instances-instance-users-put.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Resetsslconfig
  description: Deletes all client certificates and generates a new server SSL certificate
    for the instance. The changes will not take effect until the instance is restarted.
    Existing instances without a server certificate will need to call this once to
    set a server certificate.
  image: ""
  humanURL: https://cloud.google.com/sql/
  baseURL: http:://www.googleapis.com//sql/v1beta4
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projects-project-instances-instance-resetsslconfig-post.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projects-project-instances-instance-resetsslconfig-post-postman.md
x-common:
- type: x-change-log
  url: https://cloud.google.com/sql/docs/release-notes
- type: x-code
  url: https://cloud.google.com/sql/docs/admin-api/libraries
- type: x-concepts
  url: https://cloud.google.com/sql/docs/postgres/concepts
- type: x-documentation
  url: https://cloud.google.com/sql/docs/
- type: x-getting-started
  url: https://cloud.google.com/sql/docs/postgres/quickstart
- type: x-guides
  url: https://cloud.google.com/sql/docs/postgres/how-to
- type: x-pricing
  url: https://cloud.google.com/sql/pricing
- type: x-service-level-agreements
  url: https://cloud.google.com/sql/sla
- type: x-support
  url: https://cloud.google.com/sql/docs/support
- type: x-website
  url: https://cloud.google.com/sql/
- type: x-change-log
  url: https://cloud.google.com/sql/docs/release-notes
- type: x-code
  url: https://cloud.google.com/sql/docs/admin-api/libraries
- type: x-concepts
  url: https://cloud.google.com/sql/docs/postgres/concepts
- type: x-documentation
  url: https://cloud.google.com/sql/docs/
- type: x-getting-started
  url: https://cloud.google.com/sql/docs/postgres/quickstart
- type: x-guides
  url: https://cloud.google.com/sql/docs/postgres/how-to
- type: x-pricing
  url: https://cloud.google.com/sql/pricing
- type: x-service-level-agreements
  url: https://cloud.google.com/sql/sla
- type: x-support
  url: https://cloud.google.com/sql/docs/support
- type: x-website
  url: https://cloud.google.com/sql/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---