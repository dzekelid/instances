swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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
  /groups/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: groupsideventsidinstances-get
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
  /me/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendareventsidinstances-get
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
  /users/{id | userPrincipalName}/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendareventsidinstances-get
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
  /groups/{id}/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: groupsidcalendareventsidinstances-get
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
  /me/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendarsideventsidinstances-get
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
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidinstances-get
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
  /me/calendargroup/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendargroupcalendarsideventsidinstances-get
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
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidinstances-get
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
  /me/calendargroups/{id}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendargroupsidcalendarsideventsidinstances-get
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
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidinstances-get
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