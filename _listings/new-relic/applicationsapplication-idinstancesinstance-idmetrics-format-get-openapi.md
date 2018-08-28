---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Applications Application  Instances Instance  Metrics. Format
  version: 1.0.0
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /applications/{application_id}/instances/{id}.{format}:
    get:
      summary: Get Applications Application  Instances  . Format
      description: |-
        This API endpoint returns a single application instance, identified by ID. The time range for summary data is the last 10 minutes.

        See our documentation for a discussion of
         summary data output.
      operationId: getApplicationsApplicationInstances.Format
      x-api-path-slug: applicationsapplication-idinstancesid-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: path
        name: id
        description: Application instance ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - ""
      - .
      - Format
  /applications/{application_id}/instances/{instance_id}/metrics.{format}:
    get:
      summary: Get Applications Application  Instances Instance  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getApplicationsApplicationInstancesInstanceMetrics.Format
      x-api-path-slug: applicationsapplication-idinstancesinstance-idmetrics-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: path
        name: instance_id
        description: Application Instance ID
        type: integer
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - Instance
      - ""
      - Metrics.
      - Format
  /applications/{application_id}/instances/{instance_id}/metrics/data.{format}:
    get:
      summary: Get Applications Application  Instances Instance  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getApplicationsApplicationInstancesInstanceMetricsData.Format
      x-api-path-slug: applicationsapplication-idinstancesinstance-idmetricsdata-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: path
        name: instance_id
        description: Application Instance ID
        type: integer
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - Instance
      - ""
      - Metrics
      - Data.
      - Format
  /applications/{application_id}/instances.{format}:
    get:
      summary: Get Applications Application  Instances. Format
      description: "This API endpoint returns a \npaginated list of instances associated
        with the given application. The time range for summary data is the last 10
        minutes.\n\nApplication instances can be filtered by hostname, or the list
        of application instance IDs.\n\nSee our documentation for a discussion and
        examples of\nusing  filters \nand summary data output."
      operationId: getApplicationsApplicationInstances.Format
      x-api-path-slug: applicationsapplication-idinstances-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: filter[hostname]
        description: Filter by server hostname
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application instance ids
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances.
      - Format
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