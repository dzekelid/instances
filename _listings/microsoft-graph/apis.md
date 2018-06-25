---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Instances
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/meeventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/usersid--userprincipalnameeventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/groupsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendar/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/mecalendareventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendar/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/usersid--userprincipalnamecalendareventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/calendar/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/groupsidcalendareventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/mecalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/usersid--userprincipalnamecalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendargroup/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/mecalendargroupcalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupcalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendargroups/{id}/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/mecalendargroupsidcalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph List Instances
  x-api-slug: microsoft-graph
  description: List instances Get the instances (occurrences) of an event for a specified
    time range. If the event is a SeriesMaster type, this returns the occurrences
    and exceptions of the event in the specified time range.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances
  tags: List, Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupsidcalendarsideventsidinstances-get-openapi.md
- name: Microsoft Graph
  x-api-slug: microsoft-graph
  description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
    cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
    Graph simplifies queries that would otherwise be more complex. You can use Microsoft
    Graph to: Access data from multiple Microsoft cloud services, including Azure
    Active Directory, Exchange Online as part of Office 365, SharePoint, OneDrive,
    OneNote, and Planner. Navigate between entities and relationships. Access intelligence
    and insights from the Microsoft cloud (for commercial users).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Instances
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/microsoft-graph/openapi.md
x-common:
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---