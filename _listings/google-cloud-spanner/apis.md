---
name: Google Cloud Spanner
x-slug: google-cloud-spanner
description: 'Cloud Spanner is the first and only relational database service that
  is both strongly consistent and horizontally scalable. With Cloud Spanner you enjoy
  all the traditional benefits of a relational database: ACID transactions, relational
  schemas (and schema changes without downtime), SQL queries, high performance, and
  high availability. But unlike any other relational database service, Cloud Spanner
  scales horizontally, to hundreds or thousands of servers, so it can handle the highest
  of transactional workloads. With automatic scaling, synchronous data replication,
  and node redundancy, Cloud Spanner delivers up to 99.999% (five 9s) of availability
  for your mission critical applications. In fact, Google&rsquo;s internal Spanner
  service has been handling millions of queries per second from many Google services
  for years.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Instances
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/apis.md
specificationVersion: "0.14"
apis:
- name: Cloud Spanner - Update Instance
  x-api-slug: v1name-patch
  description: |-
    Updates an instance, and begins allocating or releasing resources
    as requested. The returned long-running
    operation can be used to track the
    progress of updating the instance. If the named instance does not
    exist, returns `NOT_FOUND`.

    Immediately upon completion of this request:

      * For resource types for which a decrease in the instance's allocation
        has been requested, billing is based on the newly-requested level.

    Until completion of the returned operation:

      * Cancelling the operation sets its metadata's
        cancel_time, and begins
        restoring resources to their pre-request values. The operation
        is guaranteed to succeed at undoing all resource changes,
        after which point it terminates with a `CANCELLED` status.
      * All other attempts to modify the instance are rejected.
      * Reading the instance via the API continues to give the pre-request
        resource levels.

    Upon completion of the returned operation:

      * Billing begins for all successfully-allocated resources (some types
        may have lower than the requested levels).
      * All newly-reserved resources are available for serving the instance's
        tables.
      * The instance's new resource levels are readable via the API.

    The returned long-running operation will
    have a name of the format `<instance_name>/operations/<operation_id>` and
    can be used to track the instance modification.  The
    metadata field type is
    UpdateInstanceMetadata.
    The response field type is
    Instance, if successful.

    Authorization requires `spanner.instances.update` permission on
    resource name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1name-patch-openapi.md
- name: Cloud Spanner - Cancel Instance
  x-api-slug: v1namecancel-post
  description: |-
    Starts asynchronous cancellation on a long-running operation.  The server
    makes a best effort to cancel the operation, but success is not
    guaranteed.  If the server doesn't support this method, it returns
    `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
    Operations.GetOperation or
    other methods to check whether the cancellation succeeded or whether the
    operation completed despite cancellation. On successful cancellation,
    the operation is not deleted; instead, it becomes an operation with
    an Operation.error value with a google.rpc.Status.code of 1,
    corresponding to `Code.CANCELLED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1namecancel-post-openapi.md
- name: Cloud Spanner - Get Instance Configurations
  x-api-slug: v1parentinstanceconfigs-get
  description: Lists the supported instance configurations for a given project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstanceconfigs-get-openapi.md
- name: Cloud Spanner - Get Instances
  x-api-slug: v1parentinstances-get
  description: Lists all instances in the given project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstances-get-openapi.md
- name: Cloud Spanner - Create instance
  x-api-slug: v1parentinstances-post
  description: |-
    Creates an instance and begins preparing it to begin serving. The
    returned long-running operation
    can be used to track the progress of preparing the new
    instance. The instance name is assigned by the caller. If the
    named instance already exists, `CreateInstance` returns
    `ALREADY_EXISTS`.

    Immediately upon completion of this request:

      * The instance is readable via the API, with all requested attributes
        but no allocated resources. Its state is `CREATING`.

    Until completion of the returned operation:

      * Cancelling the operation renders the instance immediately unreadable
        via the API.
      * The instance can be deleted.
      * All other attempts to modify the instance are rejected.

    Upon completion of the returned operation:

      * Billing for all successfully-allocated resources begins (some types
        may have lower than the requested levels).
      * Databases can be created in the instance.
      * The instance's allocated resource levels are readable via the API.
      * The instance's state becomes `READY`.

    The returned long-running operation will
    have a name of the format `<instance_name>/operations/<operation_id>` and
    can be used to track creation of the instance.  The
    metadata field type is
    CreateInstanceMetadata.
    The response field type is
    Instance, if successful.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstances-post-openapi.md
- name: Cloud Spanner - Create instance
  x-api-slug: v1parentinstances-post
  description: |-
    Creates an instance and begins preparing it to begin serving. The
    returned long-running operation
    can be used to track the progress of preparing the new
    instance. The instance name is assigned by the caller. If the
    named instance already exists, `CreateInstance` returns
    `ALREADY_EXISTS`.

    Immediately upon completion of this request:

      * The instance is readable via the API, with all requested attributes
        but no allocated resources. Its state is `CREATING`.

    Until completion of the returned operation:

      * Cancelling the operation renders the instance immediately unreadable
        via the API.
      * The instance can be deleted.
      * All other attempts to modify the instance are rejected.

    Upon completion of the returned operation:

      * Billing for all successfully-allocated resources begins (some types
        may have lower than the requested levels).
      * Databases can be created in the instance.
      * The instance's allocated resource levels are readable via the API.
      * The instance's state becomes `READY`.

    The returned long-running operation will
    have a name of the format `<instance_name>/operations/<operation_id>` and
    can be used to track creation of the instance.  The
    metadata field type is
    CreateInstanceMetadata.
    The response field type is
    Instance, if successful.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstances-post-openapi.md
- name: Cloud Spanner - Get Instances
  x-api-slug: v1parentinstances-get
  description: Lists all instances in the given project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstances-get-openapi.md
- name: Cloud Spanner - Get Instance Configurations
  x-api-slug: v1parentinstanceconfigs-get
  description: Lists the supported instance configurations for a given project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1parentinstanceconfigs-get-openapi.md
- name: Cloud Spanner - Cancel Instance
  x-api-slug: v1namecancel-post
  description: |-
    Starts asynchronous cancellation on a long-running operation.  The server
    makes a best effort to cancel the operation, but success is not
    guaranteed.  If the server doesn't support this method, it returns
    `google.rpc.Code.UNIMPLEMENTED`.  Clients can use
    Operations.GetOperation or
    other methods to check whether the cancellation succeeded or whether the
    operation completed despite cancellation. On successful cancellation,
    the operation is not deleted; instead, it becomes an operation with
    an Operation.error value with a google.rpc.Status.code of 1,
    corresponding to `Code.CANCELLED`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1namecancel-post-openapi.md
- name: Cloud Spanner - Update Instance
  x-api-slug: v1name-patch
  description: |-
    Updates an instance, and begins allocating or releasing resources
    as requested. The returned long-running
    operation can be used to track the
    progress of updating the instance. If the named instance does not
    exist, returns `NOT_FOUND`.

    Immediately upon completion of this request:

      * For resource types for which a decrease in the instance's allocation
        has been requested, billing is based on the newly-requested level.

    Until completion of the returned operation:

      * Cancelling the operation sets its metadata's
        cancel_time, and begins
        restoring resources to their pre-request values. The operation
        is guaranteed to succeed at undoing all resource changes,
        after which point it terminates with a `CANCELLED` status.
      * All other attempts to modify the instance are rejected.
      * Reading the instance via the API continues to give the pre-request
        resource levels.

    Upon completion of the returned operation:

      * Billing begins for all successfully-allocated resources (some types
        may have lower than the requested levels).
      * All newly-reserved resources are available for serving the instance's
        tables.
      * The instance's new resource levels are readable via the API.

    The returned long-running operation will
    have a name of the format `<instance_name>/operations/<operation_id>` and
    can be used to track the instance modification.  The
    metadata field type is
    UpdateInstanceMetadata.
    The response field type is
    Instance, if successful.

    Authorization requires `spanner.instances.update` permission on
    resource name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-spanner-global-scale-consistency_2x.png
  humanURL: https://cloud.google.com/spanner/
  baseURL: ://spanner.googleapis.com//
  tags: Google APIs, Stack Network, API Service Provider, API Provider, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-cloud-spanner/v1name-patch-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.source.repositories.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.spanner.stack.network
- type: x-change-log
  url: https://cloud.google.com/spanner/docs/release-notes
- type: x-code
  url: https://cloud.google.com/spanner/docs/reference/libraries
- type: x-command-line-interfaces
  url: https://cloud.google.com/spanner/docs/gcloud-spanner
- type: x-concepts
  url: https://cloud.google.com/spanner/docs/concepts
- type: x-documentation
  url: https://cloud.google.com/spanner/docs/
- type: x-getting-started
  url: https://cloud.google.com/spanner/docs/quickstart-console
- type: x-guide
  url: https://cloud.google.com/spanner/docs/how-to
- type: x-pricing
  url: https://cloud.google.com/spanner/pricing
- type: x-rate-limits
  url: https://cloud.google.com/spanner/docs/limits
- type: x-schema
  url: https://cloud.google.com/spanner/docs/information-schema
- type: x-service-level-agreements
  url: https://cloud.google.com/spanner/sla
- type: x-support
  url: https://cloud.google.com/spanner/docs/support
- type: x-website
  url: https://cloud.google.com/spanner/
- type: x-white-papers
  url: https://cloud.google.com/spanner/docs/whitepapers
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---