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
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud SQL API Get Projects Project Instances
  x-api-slug: google-cloud-sql-api
  description: Lists instances under a given project in the alphabetical order of
    the instance name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances
  tags: Projects, Project, Instances
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances
  x-api-slug: google-cloud-sql-api
  description: Creates a new Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances
  tags: Projects, Project, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstances-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance
  x-api-slug: google-cloud-sql-api
  description: Deletes a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}
  tags: Projects, Project, Instances, Instance
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance
  x-api-slug: google-cloud-sql-api
  description: Retrieves a resource containing information about a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}
  tags: Projects, Project, Instances, Instance
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-get-openapi.md
- name: Google Cloud SQL API Patch Projects Project Instances Instance
  x-api-slug: google-cloud-sql-api
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.. This method supports patch semantics.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}
  tags: Projects, Project, Instances, Instance
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-patch-openapi.md
- name: Google Cloud SQL API Put Projects Project Instances Instance
  x-api-slug: google-cloud-sql-api
  description: 'Updates settings of a Cloud SQL instance. Caution: This is not a partial
    update, so you must include values for all the settings that you want to retain.
    For partial updates, use patch.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}
  tags: Put, Projects, Project, Instances, Instance
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstance-put-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Backupruns
  x-api-slug: google-cloud-sql-api
  description: Lists all backup runs associated with a given instance and configuration
    in the reverse chronological order of the enqueued time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/backupRuns
  tags: Projects, Project, Instances, Instance, Backupruns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Backupruns
  x-api-slug: google-cloud-sql-api
  description: Creates a new backup run on demand. This method is applicable only
    to Second Generation instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/backupRuns
  tags: Projects, Project, Instances, Instance, Backupruns
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackupruns-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance Backupruns
  x-api-slug: google-cloud-sql-api
  description: Deletes the backup taken by a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/backupRuns/{id}
  tags: Projects, Project, Instances, Instance, Backupruns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Backupruns
  x-api-slug: google-cloud-sql-api
  description: Retrieves a resource containing information about a backup run.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/backupRuns/{id}
  tags: Projects, Project, Instances, Instance, Backupruns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancebackuprunsid-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Clone
  x-api-slug: google-cloud-sql-api
  description: Creates a Cloud SQL instance as a clone of the source instance. The
    API is not ready for Second Generation instances yet.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/clone
  tags: Projects, Project, Instances, Instance, Clone
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceclone-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Createephemeral
  x-api-slug: google-cloud-sql-api
  description: Generates a short-lived X509 certificate containing the provided public
    key and signed by a private key specific to the target instance. Users may use
    the certificate to authenticate as themselves when connecting to the database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/createEphemeral
  tags: Projects, Project, Instances, Instance, Createephemeral
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancecreateephemeral-post-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Databases
  x-api-slug: google-cloud-sql-api
  description: Lists databases in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases
  tags: Projects, Project, Instances, Instance, Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Databases
  x-api-slug: google-cloud-sql-api
  description: Inserts a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases
  tags: Projects, Project, Instances, Instance, Databases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabases-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance Databases
    Database
  x-api-slug: google-cloud-sql-api
  description: Deletes a database from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Retrieves a resource containing information about a database inside
    a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-get-openapi.md
- name: Google Cloud SQL API Patch Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-patch-openapi.md
- name: Google Cloud SQL API Put Projects Project Instances Instance Databases Database
  x-api-slug: google-cloud-sql-api
  description: Updates a resource containing information about a database inside a
    Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/databases/{database}
  tags: Put, Projects, Project, Instances, Instance, Databases, Database
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancedatabasesdatabase-put-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Export
  x-api-slug: google-cloud-sql-api
  description: Exports data from a Cloud SQL instance to a Google Cloud Storage bucket
    as a MySQL dump file.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/export
  tags: Projects, Project, Instances, Instance, Export
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceexport-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Failover
  x-api-slug: google-cloud-sql-api
  description: Failover the instance to its failover replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/failover
  tags: Projects, Project, Instances, Instance, Failover
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancefailover-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Import
  x-api-slug: google-cloud-sql-api
  description: Imports data into a Cloud SQL instance from a MySQL dump file in Google
    Cloud Storage.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/import
  tags: Projects, Project, Instances, Instance, Import
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceimport-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Promotereplica
  x-api-slug: google-cloud-sql-api
  description: Promotes the read replica instance to be a stand-alone Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/promoteReplica
  tags: Projects, Project, Instances, Instance, Promotereplica
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancepromotereplica-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Resetsslconfig
  x-api-slug: google-cloud-sql-api
  description: Deletes all client certificates and generates a new server SSL certificate
    for the instance. The changes will not take effect until the instance is restarted.
    Existing instances without a server certificate will need to call this once to
    set a server certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/resetSslConfig
  tags: Projects, Project, Instances, Instance, Resetsslconfig
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceresetsslconfig-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Restart
  x-api-slug: google-cloud-sql-api
  description: Restarts a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/restart
  tags: Projects, Project, Instances, Instance, Restart
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestart-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Restorebackup
  x-api-slug: google-cloud-sql-api
  description: Restores a backup of a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/restoreBackup
  tags: Projects, Project, Instances, Instance, Restorebackup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancerestorebackup-post-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Sslcerts
  x-api-slug: google-cloud-sql-api
  description: Lists all of the current SSL certificates for the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/sslCerts
  tags: Projects, Project, Instances, Instance, Sslcerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Sslcerts
  x-api-slug: google-cloud-sql-api
  description: Creates an SSL certificate and returns it along with the private key
    and server certificate authority. The new certificate will not be usable until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/sslCerts
  tags: Projects, Project, Instances, Instance, Sslcerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcerts-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance Sslcerts Sha1fingerprint
  x-api-slug: google-cloud-sql-api
  description: Deletes the SSL certificate. The change will not take effect until
    the instance is restarted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/sslCerts/{sha1Fingerprint}
  tags: Projects, Project, Instances, Instance, Sslcerts, Sha1fingerprint
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Sslcerts Sha1fingerprint
  x-api-slug: google-cloud-sql-api
  description: Retrieves a particular SSL certificate. Does not include the private
    key (required for usage). The private key must be saved from the response to initial
    creation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/sslCerts/{sha1Fingerprint}
  tags: Projects, Project, Instances, Instance, Sslcerts, Sha1fingerprint
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancesslcertssha1fingerprint-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Startreplica
  x-api-slug: google-cloud-sql-api
  description: Starts the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/startReplica
  tags: Projects, Project, Instances, Instance, Startreplica
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestartreplica-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Stopreplica
  x-api-slug: google-cloud-sql-api
  description: Stops the replication in the read replica instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/stopReplica
  tags: Projects, Project, Instances, Instance, Stopreplica
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancestopreplica-post-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Truncatelog
  x-api-slug: google-cloud-sql-api
  description: Truncate MySQL general and slow query log tables
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/truncateLog
  tags: Projects, Project, Instances, Instance, Truncatelog
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstancetruncatelog-post-openapi.md
- name: Google Cloud SQL API Delete Projects Project Instances Instance Users
  x-api-slug: google-cloud-sql-api
  description: Deletes a user from a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/users
  tags: Projects, Project, Instances, Instance, Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-delete-openapi.md
- name: Google Cloud SQL API Get Projects Project Instances Instance Users
  x-api-slug: google-cloud-sql-api
  description: Lists users in the specified Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/users
  tags: Projects, Project, Instances, Instance, Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-get-openapi.md
- name: Google Cloud SQL API Add Projects Project Instances Instance Users
  x-api-slug: google-cloud-sql-api
  description: Creates a new user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/users
  tags: Projects, Project, Instances, Instance, Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-post-openapi.md
- name: Google Cloud SQL API Put Projects Project Instances Instance Users
  x-api-slug: google-cloud-sql-api
  description: Updates an existing user in a Cloud SQL instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4//projects/{project}/instances/{instance}/users
  tags: Put, Projects, Project, Instances, Instance, Users
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/projectsprojectinstancesinstanceusers-put-openapi.md
- name: Google Cloud SQL API
  x-api-slug: google-cloud-sql-api
  description: Cloud SQL is a fully-managed database service that makes it easy to
    set up, maintain, manage, and administer your relational PostgreSQL BETA and MySQL
    databases in the cloud. Cloud SQL offers high performance, scalability, and convenience.
    Hosted on Google Cloud Platform, Cloud SQL provides a database infrastructure
    for applications running anywhere.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-cloud-sql-lead-2x.png
  humanURL: https://cloud.google.com/sql/
  baseURL: ://www.googleapis.com//sql/v1beta4
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-sql/openapi.md
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
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---