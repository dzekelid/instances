---
name: Google Cloud SQL
x-slug: google-cloud-sql
description: Cloud SQL is a fully-managed database service that makes it easy to set
  up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL databases
  in the cloud. Cloud SQL offers high performance, scalability, and convenience. Hosted
  on Google Cloud Platform, Cloud SQL provides a database infrastructure for applications
  running anywhere.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Instances
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/apis.md
specificationVersion: "0.14"
apis:
- name: Cloud SQL Administration - Get Projects Project Instances
  x-api-slug: projectsprojectinstances-get
  description: Lists instances under a given project in the alphabetical order of
    the instance name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances
  x-api-slug: projectsprojectinstances-post
  description: Creates a new Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-delete
  description: Deletes a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-get
  description: Retrieves a resource containing information about a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-patch
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.. This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-patch-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-put
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-put-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-get
  description: Lists all backup runs associated with a given instance and configuration
    in the reverse chronological order of the enqueued time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-post
  description: Creates a new backup run on demand. This method is applicable only
    to Second Generation instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-delete
  description: Deletes the backup taken by a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-get
  description: Retrieves a resource containing information about a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Clone
  x-api-slug: projectsprojectinstancesinstanceclone-post
  description: Creates a Cloud SQL instance as a clone of the source instance. The
    API is not ready for Second Generation instances yet.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceclone-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Createephemeral
  x-api-slug: projectsprojectinstancesinstancecreateephemeral-post
  description: Generates a short-lived X509 certificate containing the provided public
    key and signed by a private key specific to the target instance. Users may use
    the certificate to authenticate as themselves when connecting to the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancecreateephemeral-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-get
  description: Lists databases in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-post
  description: Inserts a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
  description: Deletes a database from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-get
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-patch
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-patch-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-put
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-put-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Export
  x-api-slug: projectsprojectinstancesinstanceexport-post
  description: Exports data from a Cloud SQL instance to a Google Cloud Storage bucket
    as a MySQL dump file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceexport-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Failover
  x-api-slug: projectsprojectinstancesinstancefailover-post
  description: Failover the instance to its failover replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancefailover-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Import
  x-api-slug: projectsprojectinstancesinstanceimport-post
  description: Imports data into a Cloud SQL instance from a MySQL dump file in Google
    Cloud Storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceimport-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Promotereplica
  x-api-slug: projectsprojectinstancesinstancepromotereplica-post
  description: Promotes the read replica instance to be a stand-alone Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Resetsslconfig
  x-api-slug: projectsprojectinstancesinstanceresetsslconfig-post
  description: Deletes all client certificates and generates a new server SSL certificate
    for the instance. The changes will not take effect until the instance is restarted.
    Existing instances without a server certificate will need to call this once to
    set a server certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restart
  x-api-slug: projectsprojectinstancesinstancerestart-post
  description: Restarts a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restorebackup
  x-api-slug: projectsprojectinstancesinstancerestorebackup-post
  description: Restores a backup of a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestorebackup-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-get
  description: Lists all of the current SSL certificates for the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-post
  description: Creates an SSL certificate and returns it along with the private key
    and server certificate authority. The new certificate will not be usable until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-delete
  description: Deletes the SSL certificate. The change will not take effect until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-get
  description: Retrieves a particular SSL certificate. Does not include the private
    key (required for usage). The private key must be saved from the response to initial
    creation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Startreplica
  x-api-slug: projectsprojectinstancesinstancestartreplica-post
  description: Starts the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Stopreplica
  x-api-slug: projectsprojectinstancesinstancestopreplica-post
  description: Stops the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Truncatelog
  x-api-slug: projectsprojectinstancesinstancetruncatelog-post
  description: Truncate MySQL general and slow query log tables
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancetruncatelog-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-delete
  description: Deletes a user from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-get
  description: Lists users in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-post
  description: Creates a new user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-post-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-put
  description: Updates an existing user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-put-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-delete
  description: Deletes a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-get
  description: Retrieves a resource containing information about a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-patch
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.. This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-patch-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-put
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-put-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-get
  description: Lists all backup runs associated with a given instance and configuration
    in the reverse chronological order of the enqueued time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-post
  description: Creates a new backup run on demand. This method is applicable only
    to Second Generation instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-delete
  description: Deletes the backup taken by a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-get
  description: Retrieves a resource containing information about a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Clone
  x-api-slug: projectsprojectinstancesinstanceclone-post
  description: Creates a Cloud SQL instance as a clone of the source instance. The
    API is not ready for Second Generation instances yet.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceclone-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Createephemeral
  x-api-slug: projectsprojectinstancesinstancecreateephemeral-post
  description: Generates a short-lived X509 certificate containing the provided public
    key and signed by a private key specific to the target instance. Users may use
    the certificate to authenticate as themselves when connecting to the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancecreateephemeral-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-get
  description: Lists databases in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-post
  description: Inserts a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
  description: Deletes a database from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-get
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-patch
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-patch-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-put
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-put-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Export
  x-api-slug: projectsprojectinstancesinstanceexport-post
  description: Exports data from a Cloud SQL instance to a Google Cloud Storage bucket
    as a MySQL dump file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceexport-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Failover
  x-api-slug: projectsprojectinstancesinstancefailover-post
  description: Failover the instance to its failover replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancefailover-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Import
  x-api-slug: projectsprojectinstancesinstanceimport-post
  description: Imports data into a Cloud SQL instance from a MySQL dump file in Google
    Cloud Storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceimport-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Promotereplica
  x-api-slug: projectsprojectinstancesinstancepromotereplica-post
  description: Promotes the read replica instance to be a stand-alone Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Resetsslconfig
  x-api-slug: projectsprojectinstancesinstanceresetsslconfig-post
  description: Deletes all client certificates and generates a new server SSL certificate
    for the instance. The changes will not take effect until the instance is restarted.
    Existing instances without a server certificate will need to call this once to
    set a server certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restart
  x-api-slug: projectsprojectinstancesinstancerestart-post
  description: Restarts a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restorebackup
  x-api-slug: projectsprojectinstancesinstancerestorebackup-post
  description: Restores a backup of a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestorebackup-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-get
  description: Lists all of the current SSL certificates for the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-post
  description: Creates an SSL certificate and returns it along with the private key
    and server certificate authority. The new certificate will not be usable until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-delete
  description: Deletes the SSL certificate. The change will not take effect until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-get
  description: Retrieves a particular SSL certificate. Does not include the private
    key (required for usage). The private key must be saved from the response to initial
    creation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Startreplica
  x-api-slug: projectsprojectinstancesinstancestartreplica-post
  description: Starts the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Stopreplica
  x-api-slug: projectsprojectinstancesinstancestopreplica-post
  description: Stops the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Truncatelog
  x-api-slug: projectsprojectinstancesinstancetruncatelog-post
  description: Truncate MySQL general and slow query log tables
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancetruncatelog-post-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-delete
  description: Deletes a user from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-get
  description: Lists users in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-post
  description: Creates a new user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-post-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-put
  description: Updates an existing user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-put-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-put
  description: Updates an existing user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-put-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-post
  description: Creates a new user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-get
  description: Lists users in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Users
  x-api-slug: projectsprojectinstancesinstanceusers-delete
  description: Deletes a user from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Truncatelog
  x-api-slug: projectsprojectinstancesinstancetruncatelog-post
  description: Truncate MySQL general and slow query log tables
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancetruncatelog-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Stopreplica
  x-api-slug: projectsprojectinstancesinstancestopreplica-post
  description: Stops the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Startreplica
  x-api-slug: projectsprojectinstancesinstancestartreplica-post
  description: Starts the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-get
  description: Retrieves a particular SSL certificate. Does not include the private
    key (required for usage). The private key must be saved from the response to initial
    creation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Sslcerts
    Sha1fingerprint
  x-api-slug: projectsprojectinstancesinstancesslcertssha1fingerprint-delete
  description: Deletes the SSL certificate. The change will not take effect until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-post
  description: Creates an SSL certificate and returns it along with the private key
    and server certificate authority. The new certificate will not be usable until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Sslcerts
  x-api-slug: projectsprojectinstancesinstancesslcerts-get
  description: Lists all of the current SSL certificates for the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restorebackup
  x-api-slug: projectsprojectinstancesinstancerestorebackup-post
  description: Restores a backup of a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestorebackup-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Restart
  x-api-slug: projectsprojectinstancesinstancerestart-post
  description: Restarts a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Resetsslconfig
  x-api-slug: projectsprojectinstancesinstanceresetsslconfig-post
  description: Deletes all client certificates and generates a new server SSL certificate
    for the instance. The changes will not take effect until the instance is restarted.
    Existing instances without a server certificate will need to call this once to
    set a server certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Promotereplica
  x-api-slug: projectsprojectinstancesinstancepromotereplica-post
  description: Promotes the read replica instance to be a stand-alone Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Import
  x-api-slug: projectsprojectinstancesinstanceimport-post
  description: Imports data into a Cloud SQL instance from a MySQL dump file in Google
    Cloud Storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceimport-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Failover
  x-api-slug: projectsprojectinstancesinstancefailover-post
  description: Failover the instance to its failover replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancefailover-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Export
  x-api-slug: projectsprojectinstancesinstanceexport-post
  description: Exports data from a Cloud SQL instance to a Google Cloud Storage bucket
    as a MySQL dump file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceexport-post-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-put
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-put-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-patch
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-patch-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-get
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Databases
    Database
  x-api-slug: projectsprojectinstancesinstancedatabasesdatabase-delete
  description: Deletes a database from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-post
  description: Inserts a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Databases
  x-api-slug: projectsprojectinstancesinstancedatabases-get
  description: Lists databases in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Createephemeral
  x-api-slug: projectsprojectinstancesinstancecreateephemeral-post
  description: Generates a short-lived X509 certificate containing the provided public
    key and signed by a private key specific to the target instance. Users may use
    the certificate to authenticate as themselves when connecting to the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancecreateephemeral-post-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Clone
  x-api-slug: projectsprojectinstancesinstanceclone-post
  description: Creates a Cloud SQL instance as a clone of the source instance. The
    API is not ready for Second Generation instances yet.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceclone-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-get
  description: Retrieves a resource containing information about a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackuprunsid-delete
  description: Deletes the backup taken by a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-openapi.md
- name: Cloud SQL Administration - Add Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-post
  description: Creates a new backup run on demand. This method is applicable only
    to Second Generation instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-post-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance Backupruns
  x-api-slug: projectsprojectinstancesinstancebackupruns-get
  description: Lists all backup runs associated with a given instance and configuration
    in the reverse chronological order of the enqueued time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-openapi.md
- name: Cloud SQL Administration - Put Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-put
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-put-openapi.md
- name: Cloud SQL Administration - Patch Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-patch
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.. This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-patch-openapi.md
- name: Cloud SQL Administration - Get Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-get
  description: Retrieves a resource containing information about a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-openapi.md
- name: Cloud SQL Administration - Delete Projects Project Instances Instance
  x-api-slug: projectsprojectinstancesinstance-delete
  description: Deletes a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.spanner.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.sql.stack.network
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