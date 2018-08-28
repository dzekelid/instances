---
swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 0
info:
  title: AWS Pinpoint API Segment Version Instance
  version: 1.0.0
  description: Use the GET method to request information about a segment version.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/campaigns/campaign-id:
    get:
      summary: Campaign Instance
      description: Use the GET method to request information about a campaign.
      operationId: getCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Update Campaign Instance
      description: Use the PUT method to update a campaign.
      operationId: updateCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-put
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
    delete:
      summary: Delete Campaign Instance
      description: Use the DELETE method to delete a campaign.
      operationId: deleteCampaign
      x-api-path-slug: appsapplicationidcampaignscampaignid-delete
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /apps/application-id/campaigns/campaign-id/versions/version:
    get:
      summary: Campaign Version Instance
      description: Use the GET method to request information about a campaign version.
      operationId: campaignVersionInstance
      x-api-path-slug: appsapplicationidcampaignscampaignidversionsversion-get
      parameters:
      - in: header
        name: accept
        description: 'Specify the media type you will accept as a response:  application/json
          ??? A JSON response body'
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Campaign Version
  /apps/application-id/endpoints/endpoint-id:
    get:
      summary: Endpoint Instance
      description: Use the GET method to request information about an endpoint.
      operationId: getEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-get
      responses:
        200:
          description: OK
      tags:
      - Endpoint
    put:
      summary: Update Endpoint Instance
      description: Use the PUT method to update an endpoint.
      operationId: updateEndpointInstance
      x-api-path-slug: appsapplicationidendpointsendpointid-put
      responses:
        200:
          description: OK
      tags:
      - Endpoint
  /apps/application-id/jobs/import/{job-id}:
    get:
      summary: Import Job Instance
      description: Use the GET method to request information about an import job.
      operationId: importJobInstance
      x-api-path-slug: appsapplicationidjobsimportjobid-get
      parameters:
      - in: path
        name: job-id
        description: The job id
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Import Job
  /apps/application-id/segments/segment-id:
    get:
      summary: Segment Instance
      description: Use the GET method to request information about a segment.
      operationId: getSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-get
      responses:
        200:
          description: OK
      tags:
      - Segments
    put:
      summary: Segment Instance
      description: Use the PUT method to update a segment.
      operationId: updateSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-put
      responses:
        200:
          description: OK
      tags:
      - Segments
    delete:
      summary: Segment Instance
      description: Use the DELETE method to delete a segment.
      operationId: deleteSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-delete
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segments/segment-id/versions/version:
    get:
      summary: Segment Version Instance
      description: Use the GET method to request information about a segment version.
      operationId: getSegmentVersionInstance
      x-api-path-slug: appsapplicationidsegmentssegmentidversionsversion-get
      responses:
        200:
          description: OK
      tags:
      - Segments
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