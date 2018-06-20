---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Instances
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: meeventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnameeventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
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