---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Set  Zone Managed Instance Template
  description: Specifies the instance template to use when creating new instances
    in this group. The templates for existing instances in the group do not change
    unless you recreate them.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/aggregated/instances:
    get:
      summary: Get Instances
      description: Retrieves aggregated list of instances.
      operationId: compute.instances.aggregatedList
      x-api-path-slug: projectaggregatedinstances-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
      - Aggregation
  /{project}/moveInstance:
    post:
      summary: Move Instance
      description: Moves an instance and its attached persistent disks from one zone
        to another.
      operationId: compute.projects.moveInstance
      x-api-path-slug: projectmoveinstance-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/abandonInstances:
    post:
      summary: Schedule Remove instance
      description: Schedules a group action to remove the specified instances from
        the managed instance group. Abandoning an instance does not delete the instance,
        but it does remove the instance from any target pools that are applied by
        the managed instance group. This method reduces the targetSize of the managed
        instance group by the number of instances that you abandon. This operation
        is marked as DONE when the action is scheduled even if the instances have
        not yet been removed from the group. You must separately verify the status
        of the abandoning action with the listmanagedinstances method.
      operationId: compute.regionInstanceGroupManagers.abandonInstances
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerabandoninstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/deleteInstances:
    post:
      summary: Schedule Delete instance
      description: Schedules a group action to delete the specified instances in the
        managed instance group. The instances are also removed from any target pools
        of which they were a member. This method reduces the targetSize of the managed
        instance group by the number of instances that you delete. This operation
        is marked as DONE when the action is scheduled even if the instances are still
        being deleted. You must separately verify the status of the deleting action
        with the listmanagedinstances method.
      operationId: compute.regionInstanceGroupManagers.deleteInstances
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerdeleteinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/listManagedInstances:
    post:
      summary: Get instances
      description: Lists the instances in the managed instance group and instances
        that are scheduled to be created. The list includes any current actions that
        the group has scheduled for its instances.
      operationId: compute.regionInstanceGroupManagers.listManagedInstances
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
      parameters:
      - in: query
        name: filter
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: query
        name: maxResults
      - in: query
        name: order_by
      - in: query
        name: pageToken
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/recreateInstances:
    post:
      summary: Recreate Instance
      description: Schedules a group action to recreate the specified instances in
        the managed instance group. The instances are deleted and recreated using
        the current instance template for the managed instance group. This operation
        is marked as DONE when the action is scheduled even if the instances have
        not yet been recreated. You must separately verify the status of the recreating
        action with the listmanagedinstances method.
      operationId: compute.regionInstanceGroupManagers.recreateInstances
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerrecreateinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/resize:
    post:
      summary: Resize Instance
      description: Changes the intended size for the managed instance group. If you
        increase the size, the group schedules actions to create new instances using
        the current instance template. If you decrease the size, the group schedules
        delete actions on one or more instances. The resize operation is marked DONE
        when the resize actions are scheduled even if the group has not yet added
        or deleted any instances. You must separately verify the status of the creating
        or deleting actions with the listmanagedinstances method.
      operationId: compute.regionInstanceGroupManagers.resize
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerresize-post
      parameters:
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      - in: query
        name: size
        description: Number of instances that should exist in this instance group
          manager
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/setInstanceTemplate:
    post:
      summary: Set Instance Template
      description: Sets the instance template to use when creating new instances or
        recreating instances in this group. Existing instances are not affected.
      operationId: compute.regionInstanceGroupManagers.setInstanceTemplate
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}/setTargetPools:
    post:
      summary: Set Instance Target Pools
      description: Modifies the target pools to which all new instances in this group
        are assigned. Existing instances in the group are not affected.
      operationId: compute.regionInstanceGroupManagers.setTargetPools
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersettargetpools-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/regions/{region}/instanceGroups/{instanceGroup}/listInstances:
    post:
      summary: List Instances
      description: Lists the instances in the specified instance group and displays
        information about the named ports. Depending on the specified options, this
        method can list all instances or only the instances that are running.
      operationId: compute.regionInstanceGroups.listInstances
      x-api-path-slug: projectregionsregioninstancegroupsinstancegrouplistinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: path
        name: instanceGroup
        description: Name of the regional instance group for which we want to list
          the instances
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/setCommonInstanceMetadata:
    post:
      summary: Set Common Instance Metadata
      description: Sets metadata common to all instances within the specified project
        using the data included in the request.
      operationId: compute.projects.setCommonInstanceMetadata
      x-api-path-slug: projectsetcommoninstancemetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/abandonInstances:
    post:
      summary: Schedule Action to Abandon Instance
      description: Schedules a group action to remove the specified instances from
        the managed instance group. Abandoning an instance does not delete the instance,
        but it does remove the instance from any target pools that are applied by
        the managed instance group. This method reduces the targetSize of the managed
        instance group by the number of instances that you abandon. This operation
        is marked as DONE when the action is scheduled even if the instances have
        not yet been removed from the group. You must separately verify the status
        of the abandoning action with the listmanagedinstances method.
      operationId: compute.instanceGroupManagers.abandonInstances
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerabandoninstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/deleteInstances:
    post:
      summary: Schedule Action to Delete Instance
      description: Schedules a group action to delete the specified instances in the
        managed instance group. The instances are also removed from any target pools
        of which they were a member. This method reduces the targetSize of the managed
        instance group by the number of instances that you delete. This operation
        is marked as DONE when the action is scheduled even if the instances are still
        being deleted. You must separately verify the status of the deleting action
        with the listmanagedinstances method.
      operationId: compute.instanceGroupManagers.deleteInstances
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerdeleteinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/listManagedInstances:
    post:
      summary: Get Zone Managed Instances
      description: Lists all of the instances in the managed instance group. Each
        instance in the list has a currentAction, which indicates the action that
        the managed instance group is performing on the instance. For example, if
        the group is still creating an instance, the currentAction is CREATING. If
        a previous action failed, the list displays the errors for that failed action.
      operationId: compute.instanceGroupManagers.listManagedInstances
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
      parameters:
      - in: query
        name: filter
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: query
        name: maxResults
      - in: query
        name: order_by
      - in: query
        name: pageToken
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/recreateInstances:
    post:
      summary: Schedule Recreate of Instance
      description: Schedules a group action to recreate the specified instances in
        the managed instance group. The instances are deleted and recreated using
        the current instance template for the managed instance group. This operation
        is marked as DONE when the action is scheduled even if the instances have
        not yet been recreated. You must separately verify the status of the recreating
        action with the listmanagedinstances method.
      operationId: compute.instanceGroupManagers.recreateInstances
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerrecreateinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/resize:
    post:
      summary: Schedule Resize of Instance
      description: Resizes the managed instance group. If you increase the size, the
        group creates new instances using the current instance template. If you decrease
        the size, the group deletes instances. The resize operation is marked DONE
        when the resize actions are scheduled even if the group has not yet added
        or deleted any instances. You must separately verify the status of the creating
        or deleting actions with the listmanagedinstances method.
      operationId: compute.instanceGroupManagers.resize
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerresize-post
      parameters:
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: query
        name: size
        description: The number of running instances that the managed instance group
          should maintain at any given time
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/setInstanceTemplate:
    post:
      summary: Set  Zone Managed Instance Template
      description: Specifies the instance template to use when creating new instances
        in this group. The templates for existing instances in the group do not change
        unless you recreate them.
      operationId: compute.instanceGroupManagers.setInstanceTemplate
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instanceGroupManagers/{instanceGroupManager}/setTargetPools:
    post:
      summary: Modify  Zone Managed Instance Target Pool
      description: Modifies the target pools to which all instances in this managed
        instance group are assigned. The target pools automatically apply to all of
        the instances in the managed instance group. This operation is marked DONE
        when you make the request even if the instances have not yet been added to
        their target pools. The change might take some time to apply to all of the
        instances in the group depending on the size of the group.
      operationId: compute.instanceGroupManagers.setTargetPools
      x-api-path-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersettargetpools-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroupManager
        description: The name of the managed instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the managed instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances:
    get:
      summary: Get Zone Instances
      description: Retrieves the list of instances contained within the specified
        zone.
      operationId: compute.instances.list
      x-api-path-slug: projectzoneszoneinstances-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
    post:
      summary: Create Zone Instance
      description: Creates an instance resource in the specified project using the
        data included in the request.
      operationId: compute.instances.insert
      x-api-path-slug: projectzoneszoneinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}:
    delete:
      summary: Delete Zone Instance
      description: Deletes the specified Instance resource. For more information,
        see Stopping or Deleting an Instance.
      operationId: compute.instances.delete
      x-api-path-slug: projectzoneszoneinstancesinstance-delete
      parameters:
      - in: path
        name: instance
        description: Name of the instance resource to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
    get:
      summary: Get Zone Instance
      description: Returns the specified Instance resource. Get a list of available
        instances by making a list() request.
      operationId: compute.instances.get
      x-api-path-slug: projectzoneszoneinstancesinstance-get
      parameters:
      - in: path
        name: instance
        description: Name of the instance resource to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/addAccessConfig:
    post:
      summary: Add Access to Zone Instance
      description: Adds an access config to an instance's network interface.
      operationId: compute.instances.addAccessConfig
      x-api-path-slug: projectzoneszoneinstancesinstanceaddaccessconfig-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: The instance name for this request
      - in: query
        name: networkInterface
        description: The name of the network interface to add to this instance
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/deleteAccessConfig:
    post:
      summary: Delete Access to Zone Instance
      description: Deletes an access config from an instance's network interface.
      operationId: compute.instances.deleteAccessConfig
      x-api-path-slug: projectzoneszoneinstancesinstancedeleteaccessconfig-post
      parameters:
      - in: query
        name: accessConfig
        description: The name of the access config to delete
      - in: path
        name: instance
        description: The instance name for this request
      - in: query
        name: networkInterface
        description: The name of the network interface
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/detachDisk:
    post:
      summary: Detach Disk from Zone Instance
      description: Detaches a disk from an instance.
      operationId: compute.instances.detachDisk
      x-api-path-slug: projectzoneszoneinstancesinstancedetachdisk-post
      parameters:
      - in: query
        name: deviceName
        description: Disk device name to detach
      - in: path
        name: instance
        description: Instance name
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/reset:
    post:
      summary: Reset Zone Instance
      description: Performs a hard reset on the instance.
      operationId: compute.instances.reset
      x-api-path-slug: projectzoneszoneinstancesinstancereset-post
      parameters:
      - in: path
        name: instance
        description: Name of the instance scoping this request
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/serialPort:
    get:
      summary: Get Zone Instance Serial Port
      description: Returns the specified instance's serial port output.
      operationId: compute.instances.getSerialPortOutput
      x-api-path-slug: projectzoneszoneinstancesinstanceserialport-get
      parameters:
      - in: path
        name: instance
        description: Name of the instance scoping this request
      - in: query
        name: port
        description: Specifies which COM or serial port to retrieve data from
      - in: path
        name: project
        description: Project ID for this request
      - in: query
        name: start
        description: Returns output starting from a specific byte position
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setDiskAutoDelete:
    post:
      summary: Set Zone Instance Disk Auto Delete
      description: Sets the auto-delete flag for a disk attached to an instance.
      operationId: compute.instances.setDiskAutoDelete
      x-api-path-slug: projectzoneszoneinstancesinstancesetdiskautodelete-post
      parameters:
      - in: query
        name: autoDelete
        description: Whether to auto-delete the disk when the instance is deleted
      - in: query
        name: deviceName
        description: The device name of the disk to modify
      - in: path
        name: instance
        description: The instance name
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setMachineType:
    post:
      summary: Set Zone Instance Machine Type
      description: Changes the machine type for a stopped instance to the machine
        type specified in the request.
      operationId: compute.instances.setMachineType
      x-api-path-slug: projectzoneszoneinstancesinstancesetmachinetype-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Name of the instance scoping this request
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setMetadata:
    post:
      summary: Set Zone Instance Metadata
      description: Sets metadata for the specified instance to the data included in
        the request.
      operationId: compute.instances.setMetadata
      x-api-path-slug: projectzoneszoneinstancesinstancesetmetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Name of the instance scoping this request
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setScheduling:
    post:
      summary: Set Zone Instance Scheduling
      description: Sets an instance's scheduling options.
      operationId: compute.instances.setScheduling
      x-api-path-slug: projectzoneszoneinstancesinstancesetscheduling-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Instance name
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setServiceAccount:
    post:
      summary: Set Zone Instance Service Account
      description: Sets the service account on the instance. For more information,
        read Changing the service account and access scopes for an instance.
      operationId: compute.instances.setServiceAccount
      x-api-path-slug: projectzoneszoneinstancesinstancesetserviceaccount-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Name of the instance resource to start
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/setTags:
    post:
      summary: Set Zone Instance Tags
      description: Sets tags for the specified instance to the data included in the
        request.
      operationId: compute.instances.setTags
      x-api-path-slug: projectzoneszoneinstancesinstancesettags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Name of the instance scoping this request
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/start:
    post:
      summary: Start Zone Instance
      description: Starts an instance that was stopped using the using the instances().stop
        method. For more information, see Restart an instance.
      operationId: compute.instances.start
      x-api-path-slug: projectzoneszoneinstancesinstancestart-post
      parameters:
      - in: path
        name: instance
        description: Name of the instance resource to start
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/startWithEncryptionKey:
    post:
      summary: Start Zone Instance with Encryption Key
      description: Starts an instance that was stopped using the using the instances().stop
        method. For more information, see Restart an instance.
      operationId: compute.instances.startWithEncryptionKey
      x-api-path-slug: projectzoneszoneinstancesinstancestartwithencryptionkey-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instance
        description: Name of the instance resource to start
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/instances/{instance}/stop:
    post:
      summary: Stop Zone Instance
      description: Stops a running instance, shutting it down cleanly, and allows
        you to restart the instance at a later time. Stopped instances do not incur
        per-minute, virtual machine usage charges while they are stopped, but any
        resources that the virtual machine is using, such as persistent disks and
        static IP addresses, will continue to be charged until they are deleted. For
        more information, see Stopping an instance.
      operationId: compute.instances.stop
      x-api-path-slug: projectzoneszoneinstancesinstancestop-post
      parameters:
      - in: path
        name: instance
        description: Name of the instance resource to stop
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/machineTypes:
    get:
      summary: Get Zone Instance Machine Types
      description: Retrieves a list of machine types available to the specified project.
      operationId: compute.machineTypes.list
      x-api-path-slug: projectzoneszonemachinetypes-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/machineTypes/{machineType}:
    get:
      summary: Get Zone Instance Machine Type
      description: Returns the specified machine type. Get a list of available machine
        types by making a list() request.
      operationId: compute.machineTypes.get
      x-api-path-slug: projectzoneszonemachinetypesmachinetype-get
      parameters:
      - in: path
        name: machineType
        description: Name of the machine type to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/operations:
    get:
      summary: Get Zone Instance Machine Operatons
      description: Retrieves a list of Operation resources contained within the specified
        zone.
      operationId: compute.zoneOperations.list
      x-api-path-slug: projectzoneszoneoperations-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone for request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/operations/{operation}:
    delete:
      summary: Delete Zone Instance Machine Operaton
      description: Deletes the specified zone-specific Operations resource.
      operationId: compute.zoneOperations.delete
      x-api-path-slug: projectzoneszoneoperationsoperation-delete
      parameters:
      - in: path
        name: operation
        description: Name of the Operations resource to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
    get:
      summary: Get Zone Instance Machine Operaton
      description: Retrieves the specified zone-specific Operations resource.
      operationId: compute.zoneOperations.get
      x-api-path-slug: projectzoneszoneoperationsoperation-get
      parameters:
      - in: path
        name: operation
        description: Name of the Operations resource to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone for this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/targetInstances:
    get:
      summary: Get Zone Target Instances
      description: Retrieves a list of TargetInstance resources available to the specified
        project and zone.
      operationId: compute.targetInstances.list
      x-api-path-slug: projectzoneszonetargetinstances-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
    post:
      summary: Create Zone Target Instance
      description: Creates a TargetInstance resource in the specified project and
        zone using the data included in the request.
      operationId: compute.targetInstances.insert
      x-api-path-slug: projectzoneszonetargetinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: Name of the zone scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
  /{project}/zones/{zone}/targetInstances/{targetInstance}:
    delete:
      summary: Delete Zone Target Instance
      description: Deletes the specified TargetInstance resource.
      operationId: compute.targetInstances.delete
      x-api-path-slug: projectzoneszonetargetinstancestargetinstance-delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: targetInstance
        description: Name of the TargetInstance resource to delete
      - in: path
        name: zone
        description: Name of the zone scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
    get:
      summary: Get Zone Target Instance
      description: Returns the specified TargetInstance resource. Get a list of available
        target instances by making a list() request.
      operationId: compute.targetInstances.get
      x-api-path-slug: projectzoneszonetargetinstancestargetinstance-get
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: targetInstance
        description: Name of the TargetInstance resource to return
      - in: path
        name: zone
        description: Name of the zone scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance
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