---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 1
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListInstances:
    get:
      summary: List Instances
      description: "Provides information about the cluster instances that Amazon EMR
        provisions on behalf of a user \n         when it creates the cluster."
      operationId: listInstances
      x-api-path-slug: actionlistinstances-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the instances
        type: string
      - in: query
        name: InstanceGroupId
        description: The identifier of the instance group for which to list the instances
        type: string
      - in: query
        name: InstanceGroupTypes
        description: The type of instance group for which to list the instances
        type: string
      - in: query
        name: InstanceStates
        description: A list of instance states that will filter the instances returned
          with this request
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instances
---