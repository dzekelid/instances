---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeregisterContainerInstance:
    get:
      summary: Deregister Container Instance
      description: Deregisters an Amazon ECS container instance from the specified
        cluster.
      operationId: deregisterContainerInstance
      x-api-path-slug: actionderegistercontainerinstance-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instance            to deregister
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          of the container instance to            deregister
        type: string
      - in: query
        name: force
        description: Forces the deregistration of the container instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=DescribeContainerInstances:
    get:
      summary: Describe Container Instances
      description: Describes Amazon EC2 Container Service container instances.
      operationId: describeContainerInstances
      x-api-path-slug: actiondescribecontainerinstances-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instances            to describe
        type: string
      - in: query
        name: containerInstances
        description: A space-separated list of container instance IDs or full Amazon
          Resource Name (ARN)            entries
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=ListContainerInstances:
    get:
      summary: List Container Instances
      description: Returns a list of container instances in a specified cluster.
      operationId: listContainerInstances
      x-api-path-slug: actionlistcontainerinstances-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instances            to list
        type: string
      - in: query
        name: filter
        description: You can filter the results of a ListContainerInstances operation
          with            cluster query language statements
        type: string
      - in: query
        name: maxResults
        description: The maximum number of container instance results returned by                ListContainerInstances
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListContainerInstances
          request where maxResults was used            and the results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
  /?Action=RegisterContainerInstance:
    get:
      summary: Register Container Instance
      description: Deregisters an Amazon ECS container instance from the specified
        cluster.
      operationId: registerContainerInstance
      x-api-path-slug: actionregistercontainerinstance-get
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
---