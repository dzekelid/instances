---
name: Google Compute Engine
x-slug: google-compute-engine
description: Google Compute Engine delivers virtual machines running in Googles innovative
  data centers and worldwide fiber network. Compute Engines tooling and workflow support
  enable scaling from single instances to global, load-balanced cloud computing.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Instances
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Compute Engine - Get Instances
  x-api-slug: projectaggregatedinstances-get
  description: Retrieves aggregated list of instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectaggregatedinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectaggregatedinstances-get-openapi.md
- name: Compute Engine - Move Instance
  x-api-slug: projectmoveinstance-post
  description: Moves an instance and its attached persistent disks from one zone to
    another.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectmoveinstance-post-openapi.md
- name: Compute Engine - Schedule Remove instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerabandoninstances-post
  description: Schedules a group action to remove the specified instances from the
    managed instance group. Abandoning an instance does not delete the instance, but
    it does remove the instance from any target pools that are applied by the managed
    instance group. This method reduces the targetSize of the managed instance group
    by the number of instances that you abandon. This operation is marked as DONE
    when the action is scheduled even if the instances have not yet been removed from
    the group. You must separately verify the status of the abandoning action with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerabandoninstances-post-openapi.md
- name: Compute Engine - Schedule Delete instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerdeleteinstances-post
  description: Schedules a group action to delete the specified instances in the managed
    instance group. The instances are also removed from any target pools of which
    they were a member. This method reduces the targetSize of the managed instance
    group by the number of instances that you delete. This operation is marked as
    DONE when the action is scheduled even if the instances are still being deleted.
    You must separately verify the status of the deleting action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerdeleteinstances-post-openapi.md
- name: Compute Engine - Get instances
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
  description: Lists the instances in the managed instance group and instances that
    are scheduled to be created. The list includes any current actions that the group
    has scheduled for its instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post-openapi.md
- name: Compute Engine - Recreate Instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerrecreateinstances-post
  description: Schedules a group action to recreate the specified instances in the
    managed instance group. The instances are deleted and recreated using the current
    instance template for the managed instance group. This operation is marked as
    DONE when the action is scheduled even if the instances have not yet been recreated.
    You must separately verify the status of the recreating action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerrecreateinstances-post-openapi.md
- name: Compute Engine - Resize Instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerresize-post
  description: Changes the intended size for the managed instance group. If you increase
    the size, the group schedules actions to create new instances using the current
    instance template. If you decrease the size, the group schedules delete actions
    on one or more instances. The resize operation is marked DONE when the resize
    actions are scheduled even if the group has not yet added or deleted any instances.
    You must separately verify the status of the creating or deleting actions with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerresize-post-openapi.md
- name: Compute Engine - Set Instance Template
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
  description: Sets the instance template to use when creating new instances or recreating
    instances in this group. Existing instances are not affected.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagersetinstancetemplate-post-openapi.md
- name: Compute Engine - Set Instance Target Pools
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersettargetpools-post
  description: Modifies the target pools to which all new instances in this group
    are assigned. Existing instances in the group are not affected.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagersettargetpools-post-openapi.md
- name: Compute Engine - List Instances
  x-api-slug: projectregionsregioninstancegroupsinstancegrouplistinstances-post
  description: Lists the instances in the specified instance group and displays information
    about the named ports. Depending on the specified options, this method can list
    all instances or only the instances that are running.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupsinstancegrouplistinstances-post-openapi.md
- name: Compute Engine - Set Common Instance Metadata
  x-api-slug: projectsetcommoninstancemetadata-post
  description: Sets metadata common to all instances within the specified project
    using the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectsetcommoninstancemetadata-post-openapi.md
- name: Compute Engine - Schedule Action to Abandon Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerabandoninstances-post
  description: Schedules a group action to remove the specified instances from the
    managed instance group. Abandoning an instance does not delete the instance, but
    it does remove the instance from any target pools that are applied by the managed
    instance group. This method reduces the targetSize of the managed instance group
    by the number of instances that you abandon. This operation is marked as DONE
    when the action is scheduled even if the instances have not yet been removed from
    the group. You must separately verify the status of the abandoning action with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerabandoninstances-post-openapi.md
- name: Compute Engine - Schedule Action to Delete Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerdeleteinstances-post
  description: Schedules a group action to delete the specified instances in the managed
    instance group. The instances are also removed from any target pools of which
    they were a member. This method reduces the targetSize of the managed instance
    group by the number of instances that you delete. This operation is marked as
    DONE when the action is scheduled even if the instances are still being deleted.
    You must separately verify the status of the deleting action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerdeleteinstances-post-openapi.md
- name: Compute Engine - Get Zone Managed Instances
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
  description: Lists all of the instances in the managed instance group. Each instance
    in the list has a currentAction, which indicates the action that the managed instance
    group is performing on the instance. For example, if the group is still creating
    an instance, the currentAction is CREATING. If a previous action failed, the list
    displays the errors for that failed action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post-openapi.md
- name: Compute Engine - Schedule Recreate of Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerrecreateinstances-post
  description: Schedules a group action to recreate the specified instances in the
    managed instance group. The instances are deleted and recreated using the current
    instance template for the managed instance group. This operation is marked as
    DONE when the action is scheduled even if the instances have not yet been recreated.
    You must separately verify the status of the recreating action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerrecreateinstances-post-openapi.md
- name: Compute Engine - Schedule Resize of Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerresize-post
  description: Resizes the managed instance group. If you increase the size, the group
    creates new instances using the current instance template. If you decrease the
    size, the group deletes instances. The resize operation is marked DONE when the
    resize actions are scheduled even if the group has not yet added or deleted any
    instances. You must separately verify the status of the creating or deleting actions
    with the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerresize-post-openapi.md
- name: Compute Engine - Set  Zone Managed Instance Template
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
  description: Specifies the instance template to use when creating new instances
    in this group. The templates for existing instances in the group do not change
    unless you recreate them.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagersetinstancetemplate-post-openapi.md
- name: Compute Engine - Modify  Zone Managed Instance Target Pool
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersettargetpools-post
  description: Modifies the target pools to which all instances in this managed instance
    group are assigned. The target pools automatically apply to all of the instances
    in the managed instance group. This operation is marked DONE when you make the
    request even if the instances have not yet been added to their target pools. The
    change might take some time to apply to all of the instances in the group depending
    on the size of the group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagersettargetpools-post-openapi.md
- name: Compute Engine - Get Zone Instances
  x-api-slug: projectzoneszoneinstances-get
  description: Retrieves the list of instances contained within the specified zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstances-get-openapi.md
- name: Compute Engine - Create Zone Instance
  x-api-slug: projectzoneszoneinstances-post
  description: Creates an instance resource in the specified project using the data
    included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstances-post-openapi.md
- name: Compute Engine - Delete Zone Instance
  x-api-slug: projectzoneszoneinstancesinstance-delete
  description: Deletes the specified Instance resource. For more information, see
    Stopping or Deleting an Instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstance-delete-openapi.md
- name: Compute Engine - Get Zone Instance
  x-api-slug: projectzoneszoneinstancesinstance-get
  description: Returns the specified Instance resource. Get a list of available instances
    by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstance-get-openapi.md
- name: Compute Engine - Add Access to Zone Instance
  x-api-slug: projectzoneszoneinstancesinstanceaddaccessconfig-post
  description: Adds an access config to an instance's network interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstanceaddaccessconfig-post-openapi.md
- name: Compute Engine - Delete Access to Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancedeleteaccessconfig-post
  description: Deletes an access config from an instance's network interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancedeleteaccessconfig-post-openapi.md
- name: Compute Engine - Detach Disk from Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancedetachdisk-post
  description: Detaches a disk from an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancedetachdisk-post-openapi.md
- name: Compute Engine - Reset Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancereset-post
  description: Performs a hard reset on the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancereset-post-openapi.md
- name: Compute Engine - Get Zone Instance Serial Port
  x-api-slug: projectzoneszoneinstancesinstanceserialport-get
  description: Returns the specified instance's serial port output.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstanceserialport-get-openapi.md
- name: Compute Engine - Set Zone Instance Disk Auto Delete
  x-api-slug: projectzoneszoneinstancesinstancesetdiskautodelete-post
  description: Sets the auto-delete flag for a disk attached to an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetdiskautodelete-post-openapi.md
- name: Compute Engine - Set Zone Instance Machine Type
  x-api-slug: projectzoneszoneinstancesinstancesetmachinetype-post
  description: Changes the machine type for a stopped instance to the machine type
    specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetmachinetype-post-openapi.md
- name: Compute Engine - Set Zone Instance Metadata
  x-api-slug: projectzoneszoneinstancesinstancesetmetadata-post
  description: Sets metadata for the specified instance to the data included in the
    request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetmetadata-post-openapi.md
- name: Compute Engine - Set Zone Instance Scheduling
  x-api-slug: projectzoneszoneinstancesinstancesetscheduling-post
  description: Sets an instance's scheduling options.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetscheduling-post-openapi.md
- name: Compute Engine - Set Zone Instance Service Account
  x-api-slug: projectzoneszoneinstancesinstancesetserviceaccount-post
  description: Sets the service account on the instance. For more information, read
    Changing the service account and access scopes for an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetserviceaccount-post-openapi.md
- name: Compute Engine - Set Zone Instance Tags
  x-api-slug: projectzoneszoneinstancesinstancesettags-post
  description: Sets tags for the specified instance to the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesettags-post-openapi.md
- name: Compute Engine - Start Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancestart-post
  description: Starts an instance that was stopped using the using the instances().stop
    method. For more information, see Restart an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestart-post-openapi.md
- name: Compute Engine - Start Zone Instance with Encryption Key
  x-api-slug: projectzoneszoneinstancesinstancestartwithencryptionkey-post
  description: Starts an instance that was stopped using the using the instances().stop
    method. For more information, see Restart an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestartwithencryptionkey-post-openapi.md
- name: Compute Engine - Stop Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancestop-post
  description: Stops a running instance, shutting it down cleanly, and allows you
    to restart the instance at a later time. Stopped instances do not incur per-minute,
    virtual machine usage charges while they are stopped, but any resources that the
    virtual machine is using, such as persistent disks and static IP addresses, will
    continue to be charged until they are deleted. For more information, see Stopping
    an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestop-post-openapi.md
- name: Compute Engine - Get Zone Instance Machine Types
  x-api-slug: projectzoneszonemachinetypes-get
  description: Retrieves a list of machine types available to the specified project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonemachinetypes-get-openapi.md
- name: Compute Engine - Get Zone Instance Machine Type
  x-api-slug: projectzoneszonemachinetypesmachinetype-get
  description: Returns the specified machine type. Get a list of available machine
    types by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonemachinetypesmachinetype-get-openapi.md
- name: Compute Engine - Get Zone Instance Machine Operatons
  x-api-slug: projectzoneszoneoperations-get
  description: Retrieves a list of Operation resources contained within the specified
    zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperations-get-openapi.md
- name: Compute Engine - Delete Zone Instance Machine Operaton
  x-api-slug: projectzoneszoneoperationsoperation-delete
  description: Deletes the specified zone-specific Operations resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperationsoperation-delete-openapi.md
- name: Compute Engine - Get Zone Instance Machine Operaton
  x-api-slug: projectzoneszoneoperationsoperation-get
  description: Retrieves the specified zone-specific Operations resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperationsoperation-get-openapi.md
- name: Compute Engine - Get Zone Target Instances
  x-api-slug: projectzoneszonetargetinstances-get
  description: Retrieves a list of TargetInstance resources available to the specified
    project and zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstances-get-openapi.md
- name: Compute Engine - Create Zone Target Instance
  x-api-slug: projectzoneszonetargetinstances-post
  description: Creates a TargetInstance resource in the specified project and zone
    using the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstances-post-openapi.md
- name: Compute Engine - Delete Zone Target Instance
  x-api-slug: projectzoneszonetargetinstancestargetinstance-delete
  description: Deletes the specified TargetInstance resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstancestargetinstance-delete-openapi.md
- name: Compute Engine - Get Zone Target Instance
  x-api-slug: projectzoneszonetargetinstancestargetinstance-get
  description: Returns the specified TargetInstance resource. Get a list of available
    target instances by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstancestargetinstance-get-openapi.md
- name: Compute Engine - Get Instances
  x-api-slug: projectaggregatedinstances-get
  description: Retrieves aggregated list of instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectaggregatedinstances-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectaggregatedinstances-get-openapi.md
- name: Compute Engine - Move Instance
  x-api-slug: projectmoveinstance-post
  description: Moves an instance and its attached persistent disks from one zone to
    another.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectmoveinstance-post-openapi.md
- name: Compute Engine - Schedule Remove instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerabandoninstances-post
  description: Schedules a group action to remove the specified instances from the
    managed instance group. Abandoning an instance does not delete the instance, but
    it does remove the instance from any target pools that are applied by the managed
    instance group. This method reduces the targetSize of the managed instance group
    by the number of instances that you abandon. This operation is marked as DONE
    when the action is scheduled even if the instances have not yet been removed from
    the group. You must separately verify the status of the abandoning action with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerabandoninstances-post-openapi.md
- name: Compute Engine - Schedule Delete instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerdeleteinstances-post
  description: Schedules a group action to delete the specified instances in the managed
    instance group. The instances are also removed from any target pools of which
    they were a member. This method reduces the targetSize of the managed instance
    group by the number of instances that you delete. This operation is marked as
    DONE when the action is scheduled even if the instances are still being deleted.
    You must separately verify the status of the deleting action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerdeleteinstances-post-openapi.md
- name: Compute Engine - Get instances
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
  description: Lists the instances in the managed instance group and instances that
    are scheduled to be created. The list includes any current actions that the group
    has scheduled for its instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post-openapi.md
- name: Compute Engine - Recreate Instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerrecreateinstances-post
  description: Schedules a group action to recreate the specified instances in the
    managed instance group. The instances are deleted and recreated using the current
    instance template for the managed instance group. This operation is marked as
    DONE when the action is scheduled even if the instances have not yet been recreated.
    You must separately verify the status of the recreating action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerrecreateinstances-post-openapi.md
- name: Compute Engine - Resize Instance
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagerresize-post
  description: Changes the intended size for the managed instance group. If you increase
    the size, the group schedules actions to create new instances using the current
    instance template. If you decrease the size, the group schedules delete actions
    on one or more instances. The resize operation is marked DONE when the resize
    actions are scheduled even if the group has not yet added or deleted any instances.
    You must separately verify the status of the creating or deleting actions with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagerresize-post-openapi.md
- name: Compute Engine - Set Instance Template
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
  description: Sets the instance template to use when creating new instances or recreating
    instances in this group. Existing instances are not affected.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagersetinstancetemplate-post-openapi.md
- name: Compute Engine - Set Instance Target Pools
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanagersettargetpools-post
  description: Modifies the target pools to which all new instances in this group
    are assigned. Existing instances in the group are not affected.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanagersettargetpools-post-openapi.md
- name: Compute Engine - List Instances
  x-api-slug: projectregionsregioninstancegroupsinstancegrouplistinstances-post
  description: Lists the instances in the specified instance group and displays information
    about the named ports. Depending on the specified options, this method can list
    all instances or only the instances that are running.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectregionsregioninstancegroupsinstancegrouplistinstances-post-openapi.md
- name: Compute Engine - Set Common Instance Metadata
  x-api-slug: projectsetcommoninstancemetadata-post
  description: Sets metadata common to all instances within the specified project
    using the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectsetcommoninstancemetadata-post-openapi.md
- name: Compute Engine - Schedule Action to Abandon Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerabandoninstances-post
  description: Schedules a group action to remove the specified instances from the
    managed instance group. Abandoning an instance does not delete the instance, but
    it does remove the instance from any target pools that are applied by the managed
    instance group. This method reduces the targetSize of the managed instance group
    by the number of instances that you abandon. This operation is marked as DONE
    when the action is scheduled even if the instances have not yet been removed from
    the group. You must separately verify the status of the abandoning action with
    the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerabandoninstances-post-openapi.md
- name: Compute Engine - Schedule Action to Delete Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerdeleteinstances-post
  description: Schedules a group action to delete the specified instances in the managed
    instance group. The instances are also removed from any target pools of which
    they were a member. This method reduces the targetSize of the managed instance
    group by the number of instances that you delete. This operation is marked as
    DONE when the action is scheduled even if the instances are still being deleted.
    You must separately verify the status of the deleting action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerdeleteinstances-post-openapi.md
- name: Compute Engine - Get Zone Managed Instances
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post
  description: Lists all of the instances in the managed instance group. Each instance
    in the list has a currentAction, which indicates the action that the managed instance
    group is performing on the instance. For example, if the group is still creating
    an instance, the currentAction is CREATING. If a previous action failed, the list
    displays the errors for that failed action.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerlistmanagedinstances-post-openapi.md
- name: Compute Engine - Schedule Recreate of Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerrecreateinstances-post
  description: Schedules a group action to recreate the specified instances in the
    managed instance group. The instances are deleted and recreated using the current
    instance template for the managed instance group. This operation is marked as
    DONE when the action is scheduled even if the instances have not yet been recreated.
    You must separately verify the status of the recreating action with the listmanagedinstances
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerrecreateinstances-post-openapi.md
- name: Compute Engine - Schedule Resize of Instance
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagerresize-post
  description: Resizes the managed instance group. If you increase the size, the group
    creates new instances using the current instance template. If you decrease the
    size, the group deletes instances. The resize operation is marked DONE when the
    resize actions are scheduled even if the group has not yet added or deleted any
    instances. You must separately verify the status of the creating or deleting actions
    with the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagerresize-post-openapi.md
- name: Compute Engine - Set  Zone Managed Instance Template
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersetinstancetemplate-post
  description: Specifies the instance template to use when creating new instances
    in this group. The templates for existing instances in the group do not change
    unless you recreate them.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagersetinstancetemplate-post-openapi.md
- name: Compute Engine - Modify  Zone Managed Instance Target Pool
  x-api-slug: projectzoneszoneinstancegroupmanagersinstancegroupmanagersettargetpools-post
  description: Modifies the target pools to which all instances in this managed instance
    group are assigned. The target pools automatically apply to all of the instances
    in the managed instance group. This operation is marked DONE when you make the
    request even if the instances have not yet been added to their target pools. The
    change might take some time to apply to all of the instances in the group depending
    on the size of the group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancegroupmanagersinstancegroupmanagersettargetpools-post-openapi.md
- name: Compute Engine - Get Zone Instances
  x-api-slug: projectzoneszoneinstances-get
  description: Retrieves the list of instances contained within the specified zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstances-get-openapi.md
- name: Compute Engine - Create Zone Instance
  x-api-slug: projectzoneszoneinstances-post
  description: Creates an instance resource in the specified project using the data
    included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstances-post-openapi.md
- name: Compute Engine - Delete Zone Instance
  x-api-slug: projectzoneszoneinstancesinstance-delete
  description: Deletes the specified Instance resource. For more information, see
    Stopping or Deleting an Instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstance-delete-openapi.md
- name: Compute Engine - Get Zone Instance
  x-api-slug: projectzoneszoneinstancesinstance-get
  description: Returns the specified Instance resource. Get a list of available instances
    by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstance-get-openapi.md
- name: Compute Engine - Add Access to Zone Instance
  x-api-slug: projectzoneszoneinstancesinstanceaddaccessconfig-post
  description: Adds an access config to an instance's network interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstanceaddaccessconfig-post-openapi.md
- name: Compute Engine - Delete Access to Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancedeleteaccessconfig-post
  description: Deletes an access config from an instance's network interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancedeleteaccessconfig-post-openapi.md
- name: Compute Engine - Detach Disk from Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancedetachdisk-post
  description: Detaches a disk from an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancedetachdisk-post-openapi.md
- name: Compute Engine - Reset Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancereset-post
  description: Performs a hard reset on the instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancereset-post-openapi.md
- name: Compute Engine - Get Zone Instance Serial Port
  x-api-slug: projectzoneszoneinstancesinstanceserialport-get
  description: Returns the specified instance's serial port output.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstanceserialport-get-openapi.md
- name: Compute Engine - Set Zone Instance Disk Auto Delete
  x-api-slug: projectzoneszoneinstancesinstancesetdiskautodelete-post
  description: Sets the auto-delete flag for a disk attached to an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetdiskautodelete-post-openapi.md
- name: Compute Engine - Set Zone Instance Machine Type
  x-api-slug: projectzoneszoneinstancesinstancesetmachinetype-post
  description: Changes the machine type for a stopped instance to the machine type
    specified in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetmachinetype-post-openapi.md
- name: Compute Engine - Set Zone Instance Metadata
  x-api-slug: projectzoneszoneinstancesinstancesetmetadata-post
  description: Sets metadata for the specified instance to the data included in the
    request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetmetadata-post-openapi.md
- name: Compute Engine - Set Zone Instance Scheduling
  x-api-slug: projectzoneszoneinstancesinstancesetscheduling-post
  description: Sets an instance's scheduling options.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetscheduling-post-openapi.md
- name: Compute Engine - Set Zone Instance Service Account
  x-api-slug: projectzoneszoneinstancesinstancesetserviceaccount-post
  description: Sets the service account on the instance. For more information, read
    Changing the service account and access scopes for an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesetserviceaccount-post-openapi.md
- name: Compute Engine - Set Zone Instance Tags
  x-api-slug: projectzoneszoneinstancesinstancesettags-post
  description: Sets tags for the specified instance to the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancesettags-post-openapi.md
- name: Compute Engine - Start Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancestart-post
  description: Starts an instance that was stopped using the using the instances().stop
    method. For more information, see Restart an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestart-post-openapi.md
- name: Compute Engine - Start Zone Instance with Encryption Key
  x-api-slug: projectzoneszoneinstancesinstancestartwithencryptionkey-post
  description: Starts an instance that was stopped using the using the instances().stop
    method. For more information, see Restart an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestartwithencryptionkey-post-openapi.md
- name: Compute Engine - Stop Zone Instance
  x-api-slug: projectzoneszoneinstancesinstancestop-post
  description: Stops a running instance, shutting it down cleanly, and allows you
    to restart the instance at a later time. Stopped instances do not incur per-minute,
    virtual machine usage charges while they are stopped, but any resources that the
    virtual machine is using, such as persistent disks and static IP addresses, will
    continue to be charged until they are deleted. For more information, see Stopping
    an instance.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneinstancesinstancestop-post-openapi.md
- name: Compute Engine - Get Zone Instance Machine Types
  x-api-slug: projectzoneszonemachinetypes-get
  description: Retrieves a list of machine types available to the specified project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonemachinetypes-get-openapi.md
- name: Compute Engine - Get Zone Instance Machine Type
  x-api-slug: projectzoneszonemachinetypesmachinetype-get
  description: Returns the specified machine type. Get a list of available machine
    types by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonemachinetypesmachinetype-get-openapi.md
- name: Compute Engine - Get Zone Instance Machine Operatons
  x-api-slug: projectzoneszoneoperations-get
  description: Retrieves a list of Operation resources contained within the specified
    zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperations-get-openapi.md
- name: Compute Engine - Delete Zone Instance Machine Operaton
  x-api-slug: projectzoneszoneoperationsoperation-delete
  description: Deletes the specified zone-specific Operations resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperationsoperation-delete-openapi.md
- name: Compute Engine - Get Zone Instance Machine Operaton
  x-api-slug: projectzoneszoneoperationsoperation-get
  description: Retrieves the specified zone-specific Operations resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszoneoperationsoperation-get-openapi.md
- name: Compute Engine - Get Zone Target Instances
  x-api-slug: projectzoneszonetargetinstances-get
  description: Retrieves a list of TargetInstance resources available to the specified
    project and zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstances-get-openapi.md
- name: Compute Engine - Create Zone Target Instance
  x-api-slug: projectzoneszonetargetinstances-post
  description: Creates a TargetInstance resource in the specified project and zone
    using the data included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstances-post-openapi.md
- name: Compute Engine - Delete Zone Target Instance
  x-api-slug: projectzoneszonetargetinstancestargetinstance-delete
  description: Deletes the specified TargetInstance resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstancestargetinstance-delete-openapi.md
- name: Compute Engine - Get Zone Target Instance
  x-api-slug: projectzoneszonetargetinstancestargetinstance-get
  description: Returns the specified TargetInstance resource. Get a list of available
    target instances by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instances/master/_listings/google-compute-engine/projectzoneszonetargetinstancestargetinstance-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.vision.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.compute.engine.stack.network
- type: x-code
  url: https://cloud.google.com/compute/docs/api/libraries
- type: x-documentation
  url: https://cloud.google.com/compute/docs/reference/latest/
- type: x-guides
  url: https://cloud.google.com/compute/docs/api/how-tos/how-tos
- type: x-rate-limits
  url: https://cloud.google.com/compute/docs/api-rate-limits
- type: x-sla
  url: https://cloud.google.com/compute/sla
- type: x-website
  url: https://cloud.google.com/compute/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---