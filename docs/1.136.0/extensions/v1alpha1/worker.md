---
permalink: /1.136.0/extensions/v1alpha1/worker/
---

# extensions.v1alpha1.worker

"Worker is a specification for a Worker resource."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withClass(class)`](#fn-specwithclass)
  * [`fn withInfrastructureProviderStatus(infrastructureProviderStatus)`](#fn-specwithinfrastructureproviderstatus)
  * [`fn withInfrastructureProviderStatusMixin(infrastructureProviderStatus)`](#fn-specwithinfrastructureproviderstatusmixin)
  * [`fn withPools(pools)`](#fn-specwithpools)
  * [`fn withPoolsMixin(pools)`](#fn-specwithpoolsmixin)
  * [`fn withProviderConfig(providerConfig)`](#fn-specwithproviderconfig)
  * [`fn withProviderConfigMixin(providerConfig)`](#fn-specwithproviderconfigmixin)
  * [`fn withRegion(region)`](#fn-specwithregion)
  * [`fn withSshPublicKey(sshPublicKey)`](#fn-specwithsshpublickey)
  * [`fn withType(type)`](#fn-specwithtype)
  * [`obj spec.pools`](#obj-specpools)
    * [`fn withAnnotations(annotations)`](#fn-specpoolswithannotations)
    * [`fn withAnnotationsMixin(annotations)`](#fn-specpoolswithannotationsmixin)
    * [`fn withArchitecture(architecture)`](#fn-specpoolswitharchitecture)
    * [`fn withDataVolumes(dataVolumes)`](#fn-specpoolswithdatavolumes)
    * [`fn withDataVolumesMixin(dataVolumes)`](#fn-specpoolswithdatavolumesmixin)
    * [`fn withKubeletDataVolumeName(kubeletDataVolumeName)`](#fn-specpoolswithkubeletdatavolumename)
    * [`fn withKubernetesVersion(kubernetesVersion)`](#fn-specpoolswithkubernetesversion)
    * [`fn withLabels(labels)`](#fn-specpoolswithlabels)
    * [`fn withLabelsMixin(labels)`](#fn-specpoolswithlabelsmixin)
    * [`fn withMachineType(machineType)`](#fn-specpoolswithmachinetype)
    * [`fn withMaxSurge(maxSurge)`](#fn-specpoolswithmaxsurge)
    * [`fn withMaxUnavailable(maxUnavailable)`](#fn-specpoolswithmaxunavailable)
    * [`fn withMaximum(maximum)`](#fn-specpoolswithmaximum)
    * [`fn withMinimum(minimum)`](#fn-specpoolswithminimum)
    * [`fn withName(name)`](#fn-specpoolswithname)
    * [`fn withNodeAgentSecretName(nodeAgentSecretName)`](#fn-specpoolswithnodeagentsecretname)
    * [`fn withPriority(priority)`](#fn-specpoolswithpriority)
    * [`fn withProviderConfig(providerConfig)`](#fn-specpoolswithproviderconfig)
    * [`fn withProviderConfigMixin(providerConfig)`](#fn-specpoolswithproviderconfigmixin)
    * [`fn withTaints(taints)`](#fn-specpoolswithtaints)
    * [`fn withTaintsMixin(taints)`](#fn-specpoolswithtaintsmixin)
    * [`fn withUpdateStrategy(updateStrategy)`](#fn-specpoolswithupdatestrategy)
    * [`fn withZones(zones)`](#fn-specpoolswithzones)
    * [`fn withZonesMixin(zones)`](#fn-specpoolswithzonesmixin)
    * [`obj spec.pools.clusterAutoscaler`](#obj-specpoolsclusterautoscaler)
      * [`fn withMaxNodeProvisionTime(maxNodeProvisionTime)`](#fn-specpoolsclusterautoscalerwithmaxnodeprovisiontime)
      * [`fn withScaleDownGpuUtilizationThreshold(scaleDownGpuUtilizationThreshold)`](#fn-specpoolsclusterautoscalerwithscaledowngpuutilizationthreshold)
      * [`fn withScaleDownUnneededTime(scaleDownUnneededTime)`](#fn-specpoolsclusterautoscalerwithscaledownunneededtime)
      * [`fn withScaleDownUnreadyTime(scaleDownUnreadyTime)`](#fn-specpoolsclusterautoscalerwithscaledownunreadytime)
      * [`fn withScaleDownUtilizationThreshold(scaleDownUtilizationThreshold)`](#fn-specpoolsclusterautoscalerwithscaledownutilizationthreshold)
    * [`obj spec.pools.dataVolumes`](#obj-specpoolsdatavolumes)
      * [`fn withEncrypted(encrypted)`](#fn-specpoolsdatavolumeswithencrypted)
      * [`fn withName(name)`](#fn-specpoolsdatavolumeswithname)
      * [`fn withSize(size)`](#fn-specpoolsdatavolumeswithsize)
      * [`fn withType(type)`](#fn-specpoolsdatavolumeswithtype)
    * [`obj spec.pools.kubeletConfig`](#obj-specpoolskubeletconfig)
      * [`fn withContainerLogMaxFiles(containerLogMaxFiles)`](#fn-specpoolskubeletconfigwithcontainerlogmaxfiles)
      * [`fn withContainerLogMaxSize(containerLogMaxSize)`](#fn-specpoolskubeletconfigwithcontainerlogmaxsize)
      * [`fn withCpuCFSQuota(cpuCFSQuota)`](#fn-specpoolskubeletconfigwithcpucfsquota)
      * [`fn withCpuManagerPolicy(cpuManagerPolicy)`](#fn-specpoolskubeletconfigwithcpumanagerpolicy)
      * [`fn withEvictionMaxPodGracePeriod(evictionMaxPodGracePeriod)`](#fn-specpoolskubeletconfigwithevictionmaxpodgraceperiod)
      * [`fn withEvictionPressureTransitionPeriod(evictionPressureTransitionPeriod)`](#fn-specpoolskubeletconfigwithevictionpressuretransitionperiod)
      * [`fn withFailSwapOn(failSwapOn)`](#fn-specpoolskubeletconfigwithfailswapon)
      * [`fn withFeatureGates(featureGates)`](#fn-specpoolskubeletconfigwithfeaturegates)
      * [`fn withFeatureGatesMixin(featureGates)`](#fn-specpoolskubeletconfigwithfeaturegatesmixin)
      * [`fn withImageGCHighThresholdPercent(imageGCHighThresholdPercent)`](#fn-specpoolskubeletconfigwithimagegchighthresholdpercent)
      * [`fn withImageGCLowThresholdPercent(imageGCLowThresholdPercent)`](#fn-specpoolskubeletconfigwithimagegclowthresholdpercent)
      * [`fn withImageMaximumGCAge(imageMaximumGCAge)`](#fn-specpoolskubeletconfigwithimagemaximumgcage)
      * [`fn withImageMinimumGCAge(imageMinimumGCAge)`](#fn-specpoolskubeletconfigwithimageminimumgcage)
      * [`fn withMaxParallelImagePulls(maxParallelImagePulls)`](#fn-specpoolskubeletconfigwithmaxparallelimagepulls)
      * [`fn withMaxPods(maxPods)`](#fn-specpoolskubeletconfigwithmaxpods)
      * [`fn withPodPidsLimit(podPidsLimit)`](#fn-specpoolskubeletconfigwithpodpidslimit)
      * [`fn withProtectKernelDefaults(protectKernelDefaults)`](#fn-specpoolskubeletconfigwithprotectkerneldefaults)
      * [`fn withRegistryBurst(registryBurst)`](#fn-specpoolskubeletconfigwithregistryburst)
      * [`fn withRegistryPullQPS(registryPullQPS)`](#fn-specpoolskubeletconfigwithregistrypullqps)
      * [`fn withSeccompDefault(seccompDefault)`](#fn-specpoolskubeletconfigwithseccompdefault)
      * [`fn withSerializeImagePulls(serializeImagePulls)`](#fn-specpoolskubeletconfigwithserializeimagepulls)
      * [`fn withStreamingConnectionIdleTimeout(streamingConnectionIdleTimeout)`](#fn-specpoolskubeletconfigwithstreamingconnectionidletimeout)
      * [`obj spec.pools.kubeletConfig.evictionHard`](#obj-specpoolskubeletconfigevictionhard)
        * [`fn withImageFSAvailable(imageFSAvailable)`](#fn-specpoolskubeletconfigevictionhardwithimagefsavailable)
        * [`fn withImageFSInodesFree(imageFSInodesFree)`](#fn-specpoolskubeletconfigevictionhardwithimagefsinodesfree)
        * [`fn withMemoryAvailable(memoryAvailable)`](#fn-specpoolskubeletconfigevictionhardwithmemoryavailable)
        * [`fn withNodeFSAvailable(nodeFSAvailable)`](#fn-specpoolskubeletconfigevictionhardwithnodefsavailable)
        * [`fn withNodeFSInodesFree(nodeFSInodesFree)`](#fn-specpoolskubeletconfigevictionhardwithnodefsinodesfree)
      * [`obj spec.pools.kubeletConfig.evictionMinimumReclaim`](#obj-specpoolskubeletconfigevictionminimumreclaim)
        * [`fn withImageFSAvailable(imageFSAvailable)`](#fn-specpoolskubeletconfigevictionminimumreclaimwithimagefsavailable)
        * [`fn withImageFSInodesFree(imageFSInodesFree)`](#fn-specpoolskubeletconfigevictionminimumreclaimwithimagefsinodesfree)
        * [`fn withMemoryAvailable(memoryAvailable)`](#fn-specpoolskubeletconfigevictionminimumreclaimwithmemoryavailable)
        * [`fn withNodeFSAvailable(nodeFSAvailable)`](#fn-specpoolskubeletconfigevictionminimumreclaimwithnodefsavailable)
        * [`fn withNodeFSInodesFree(nodeFSInodesFree)`](#fn-specpoolskubeletconfigevictionminimumreclaimwithnodefsinodesfree)
      * [`obj spec.pools.kubeletConfig.evictionSoft`](#obj-specpoolskubeletconfigevictionsoft)
        * [`fn withImageFSAvailable(imageFSAvailable)`](#fn-specpoolskubeletconfigevictionsoftwithimagefsavailable)
        * [`fn withImageFSInodesFree(imageFSInodesFree)`](#fn-specpoolskubeletconfigevictionsoftwithimagefsinodesfree)
        * [`fn withMemoryAvailable(memoryAvailable)`](#fn-specpoolskubeletconfigevictionsoftwithmemoryavailable)
        * [`fn withNodeFSAvailable(nodeFSAvailable)`](#fn-specpoolskubeletconfigevictionsoftwithnodefsavailable)
        * [`fn withNodeFSInodesFree(nodeFSInodesFree)`](#fn-specpoolskubeletconfigevictionsoftwithnodefsinodesfree)
      * [`obj spec.pools.kubeletConfig.evictionSoftGracePeriod`](#obj-specpoolskubeletconfigevictionsoftgraceperiod)
        * [`fn withImageFSAvailable(imageFSAvailable)`](#fn-specpoolskubeletconfigevictionsoftgraceperiodwithimagefsavailable)
        * [`fn withImageFSInodesFree(imageFSInodesFree)`](#fn-specpoolskubeletconfigevictionsoftgraceperiodwithimagefsinodesfree)
        * [`fn withMemoryAvailable(memoryAvailable)`](#fn-specpoolskubeletconfigevictionsoftgraceperiodwithmemoryavailable)
        * [`fn withNodeFSAvailable(nodeFSAvailable)`](#fn-specpoolskubeletconfigevictionsoftgraceperiodwithnodefsavailable)
        * [`fn withNodeFSInodesFree(nodeFSInodesFree)`](#fn-specpoolskubeletconfigevictionsoftgraceperiodwithnodefsinodesfree)
      * [`obj spec.pools.kubeletConfig.kubeReserved`](#obj-specpoolskubeletconfigkubereserved)
        * [`fn withCpu(cpu)`](#fn-specpoolskubeletconfigkubereservedwithcpu)
        * [`fn withEphemeralStorage(ephemeralStorage)`](#fn-specpoolskubeletconfigkubereservedwithephemeralstorage)
        * [`fn withMemory(memory)`](#fn-specpoolskubeletconfigkubereservedwithmemory)
        * [`fn withPid(pid)`](#fn-specpoolskubeletconfigkubereservedwithpid)
      * [`obj spec.pools.kubeletConfig.memorySwap`](#obj-specpoolskubeletconfigmemoryswap)
        * [`fn withSwapBehavior(swapBehavior)`](#fn-specpoolskubeletconfigmemoryswapwithswapbehavior)
      * [`obj spec.pools.kubeletConfig.systemReserved`](#obj-specpoolskubeletconfigsystemreserved)
        * [`fn withCpu(cpu)`](#fn-specpoolskubeletconfigsystemreservedwithcpu)
        * [`fn withEphemeralStorage(ephemeralStorage)`](#fn-specpoolskubeletconfigsystemreservedwithephemeralstorage)
        * [`fn withMemory(memory)`](#fn-specpoolskubeletconfigsystemreservedwithmemory)
        * [`fn withPid(pid)`](#fn-specpoolskubeletconfigsystemreservedwithpid)
    * [`obj spec.pools.machineControllerManager`](#obj-specpoolsmachinecontrollermanager)
      * [`fn withDisableHealthTimeout(disableHealthTimeout)`](#fn-specpoolsmachinecontrollermanagerwithdisablehealthtimeout)
      * [`fn withInPlaceUpdateTimeout(inPlaceUpdateTimeout)`](#fn-specpoolsmachinecontrollermanagerwithinplaceupdatetimeout)
      * [`fn withMachineCreationTimeout(machineCreationTimeout)`](#fn-specpoolsmachinecontrollermanagerwithmachinecreationtimeout)
      * [`fn withMachineDrainTimeout(machineDrainTimeout)`](#fn-specpoolsmachinecontrollermanagerwithmachinedraintimeout)
      * [`fn withMachineHealthTimeout(machineHealthTimeout)`](#fn-specpoolsmachinecontrollermanagerwithmachinehealthtimeout)
      * [`fn withMaxEvictRetries(maxEvictRetries)`](#fn-specpoolsmachinecontrollermanagerwithmaxevictretries)
      * [`fn withNodeConditions(nodeConditions)`](#fn-specpoolsmachinecontrollermanagerwithnodeconditions)
      * [`fn withNodeConditionsMixin(nodeConditions)`](#fn-specpoolsmachinecontrollermanagerwithnodeconditionsmixin)
    * [`obj spec.pools.machineImage`](#obj-specpoolsmachineimage)
      * [`fn withName(name)`](#fn-specpoolsmachineimagewithname)
      * [`fn withVersion(version)`](#fn-specpoolsmachineimagewithversion)
    * [`obj spec.pools.nodeTemplate`](#obj-specpoolsnodetemplate)
      * [`fn withCapacity(capacity)`](#fn-specpoolsnodetemplatewithcapacity)
      * [`fn withCapacityMixin(capacity)`](#fn-specpoolsnodetemplatewithcapacitymixin)
      * [`fn withVirtualCapacity(virtualCapacity)`](#fn-specpoolsnodetemplatewithvirtualcapacity)
      * [`fn withVirtualCapacityMixin(virtualCapacity)`](#fn-specpoolsnodetemplatewithvirtualcapacitymixin)
    * [`obj spec.pools.taints`](#obj-specpoolstaints)
      * [`fn withEffect(effect)`](#fn-specpoolstaintswitheffect)
      * [`fn withKey(key)`](#fn-specpoolstaintswithkey)
      * [`fn withTimeAdded(timeAdded)`](#fn-specpoolstaintswithtimeadded)
      * [`fn withValue(value)`](#fn-specpoolstaintswithvalue)
    * [`obj spec.pools.userDataSecretRef`](#obj-specpoolsuserdatasecretref)
      * [`fn withKey(key)`](#fn-specpoolsuserdatasecretrefwithkey)
      * [`fn withName(name)`](#fn-specpoolsuserdatasecretrefwithname)
      * [`fn withOptional(optional)`](#fn-specpoolsuserdatasecretrefwithoptional)
    * [`obj spec.pools.volume`](#obj-specpoolsvolume)
      * [`fn withEncrypted(encrypted)`](#fn-specpoolsvolumewithencrypted)
      * [`fn withName(name)`](#fn-specpoolsvolumewithname)
      * [`fn withSize(size)`](#fn-specpoolsvolumewithsize)
      * [`fn withType(type)`](#fn-specpoolsvolumewithtype)
  * [`obj spec.secretRef`](#obj-specsecretref)
    * [`fn withName(name)`](#fn-specsecretrefwithname)
    * [`fn withNamespace(namespace)`](#fn-specsecretrefwithnamespace)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Worker

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"Specification of the Worker.\nIf the object's deletion timestamp is set, this field is immutable."

### fn spec.withClass

```ts
withClass(class)
```

"Class holds the extension class used to control the responsibility for multiple provider extensions."

### fn spec.withInfrastructureProviderStatus

```ts
withInfrastructureProviderStatus(infrastructureProviderStatus)
```

"InfrastructureProviderStatus is a raw extension field that contains the provider status that has\nbeen generated by the controller responsible for the `Infrastructure` resource."

### fn spec.withInfrastructureProviderStatusMixin

```ts
withInfrastructureProviderStatusMixin(infrastructureProviderStatus)
```

"InfrastructureProviderStatus is a raw extension field that contains the provider status that has\nbeen generated by the controller responsible for the `Infrastructure` resource."

**Note:** This function appends passed data to existing values

### fn spec.withPools

```ts
withPools(pools)
```

"Pools is a list of worker pools."

### fn spec.withPoolsMixin

```ts
withPoolsMixin(pools)
```

"Pools is a list of worker pools."

**Note:** This function appends passed data to existing values

### fn spec.withProviderConfig

```ts
withProviderConfig(providerConfig)
```

"ProviderConfig is the provider specific configuration."

### fn spec.withProviderConfigMixin

```ts
withProviderConfigMixin(providerConfig)
```

"ProviderConfig is the provider specific configuration."

**Note:** This function appends passed data to existing values

### fn spec.withRegion

```ts
withRegion(region)
```

"Region is the name of the region where the worker pool should be deployed to. This field is immutable."

### fn spec.withSshPublicKey

```ts
withSshPublicKey(sshPublicKey)
```

"SSHPublicKey is the public SSH key that should be used with these workers."

### fn spec.withType

```ts
withType(type)
```

"Type contains the instance of the resource's kind."

## obj spec.pools

"Pools is a list of worker pools."

### fn spec.pools.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is a map of key/value pairs for annotations for all the `Node` objects in this worker pool."

### fn spec.pools.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is a map of key/value pairs for annotations for all the `Node` objects in this worker pool."

**Note:** This function appends passed data to existing values

### fn spec.pools.withArchitecture

```ts
withArchitecture(architecture)
```

"Architecture is the CPU architecture of the worker pool machines and machine image."

### fn spec.pools.withDataVolumes

```ts
withDataVolumes(dataVolumes)
```

"DataVolumes contains a list of additional worker volumes."

### fn spec.pools.withDataVolumesMixin

```ts
withDataVolumesMixin(dataVolumes)
```

"DataVolumes contains a list of additional worker volumes."

**Note:** This function appends passed data to existing values

### fn spec.pools.withKubeletDataVolumeName

```ts
withKubeletDataVolumeName(kubeletDataVolumeName)
```

"KubeletDataVolumeName contains the name of a dataVolume that should be used for storing kubelet state."

### fn spec.pools.withKubernetesVersion

```ts
withKubernetesVersion(kubernetesVersion)
```

"KubernetesVersion is the kubernetes version in this worker pool"

### fn spec.pools.withLabels

```ts
withLabels(labels)
```

"Labels is a map of key/value pairs for labels for all the `Node` objects in this worker pool."

### fn spec.pools.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels is a map of key/value pairs for labels for all the `Node` objects in this worker pool."

**Note:** This function appends passed data to existing values

### fn spec.pools.withMachineType

```ts
withMachineType(machineType)
```

"MachineType contains information about the machine type that should be used for this worker pool."

### fn spec.pools.withMaxSurge

```ts
withMaxSurge(maxSurge)
```

"MaxSurge is maximum number of VMs that are created during an update."

### fn spec.pools.withMaxUnavailable

```ts
withMaxUnavailable(maxUnavailable)
```

"MaxUnavailable is the maximum number of VMs that can be unavailable during an update."

### fn spec.pools.withMaximum

```ts
withMaximum(maximum)
```

"Maximum is the maximum size of the worker pool."

### fn spec.pools.withMinimum

```ts
withMinimum(minimum)
```

"Minimum is the minimum size of the worker pool."

### fn spec.pools.withName

```ts
withName(name)
```

"Name is the name of this worker pool."

### fn spec.pools.withNodeAgentSecretName

```ts
withNodeAgentSecretName(nodeAgentSecretName)
```

"NodeAgentSecretName is uniquely identifying selected aspects of the OperatingSystemConfig. If it changes, then the\nworker pool must be rolled."

### fn spec.pools.withPriority

```ts
withPriority(priority)
```

"Priority (or weight) is the importance by which this worker pool will be scaled by cluster autoscaling."

### fn spec.pools.withProviderConfig

```ts
withProviderConfig(providerConfig)
```

"ProviderConfig is a provider specific configuration for the worker pool."

### fn spec.pools.withProviderConfigMixin

```ts
withProviderConfigMixin(providerConfig)
```

"ProviderConfig is a provider specific configuration for the worker pool."

**Note:** This function appends passed data to existing values

### fn spec.pools.withTaints

```ts
withTaints(taints)
```

"Taints is a list of taints for all the `Node` objects in this worker pool."

### fn spec.pools.withTaintsMixin

```ts
withTaintsMixin(taints)
```

"Taints is a list of taints for all the `Node` objects in this worker pool."

**Note:** This function appends passed data to existing values

### fn spec.pools.withUpdateStrategy

```ts
withUpdateStrategy(updateStrategy)
```

"UpdateStrategy specifies the machine update strategy for the worker pool."

### fn spec.pools.withZones

```ts
withZones(zones)
```

"Zones contains information about availability zones for this worker pool."

### fn spec.pools.withZonesMixin

```ts
withZonesMixin(zones)
```

"Zones contains information about availability zones for this worker pool."

**Note:** This function appends passed data to existing values

## obj spec.pools.clusterAutoscaler

"ClusterAutoscaler contains the cluster autoscaler configurations for the worker pool."

### fn spec.pools.clusterAutoscaler.withMaxNodeProvisionTime

```ts
withMaxNodeProvisionTime(maxNodeProvisionTime)
```

"MaxNodeProvisionTime defines how long cluster autoscaler should wait for a node to be provisioned."

### fn spec.pools.clusterAutoscaler.withScaleDownGpuUtilizationThreshold

```ts
withScaleDownGpuUtilizationThreshold(scaleDownGpuUtilizationThreshold)
```

"ScaleDownGpuUtilizationThreshold defines the threshold in fraction (0.0 - 1.0) of gpu resources under which a node is being removed."

### fn spec.pools.clusterAutoscaler.withScaleDownUnneededTime

```ts
withScaleDownUnneededTime(scaleDownUnneededTime)
```

"ScaleDownUnneededTime defines how long a node should be unneeded before it is eligible for scale down."

### fn spec.pools.clusterAutoscaler.withScaleDownUnreadyTime

```ts
withScaleDownUnreadyTime(scaleDownUnreadyTime)
```

"ScaleDownUnreadyTime defines how long an unready node should be unneeded before it is eligible for scale down."

### fn spec.pools.clusterAutoscaler.withScaleDownUtilizationThreshold

```ts
withScaleDownUtilizationThreshold(scaleDownUtilizationThreshold)
```

"ScaleDownUtilizationThreshold defines the threshold in fraction (0.0 - 1.0) under which a node is being removed."

## obj spec.pools.dataVolumes

"DataVolumes contains a list of additional worker volumes."

### fn spec.pools.dataVolumes.withEncrypted

```ts
withEncrypted(encrypted)
```

"Encrypted determines if the volume should be encrypted."

### fn spec.pools.dataVolumes.withName

```ts
withName(name)
```

"Name of the volume to make it referenceable."

### fn spec.pools.dataVolumes.withSize

```ts
withSize(size)
```

"Size is the of the root volume."

### fn spec.pools.dataVolumes.withType

```ts
withType(type)
```

"Type is the type of the volume."

## obj spec.pools.kubeletConfig

"KubeletConfig contains the kubelet configuration for the worker pool."

### fn spec.pools.kubeletConfig.withContainerLogMaxFiles

```ts
withContainerLogMaxFiles(containerLogMaxFiles)
```

"Maximum number of container log files that can be present for a container."

### fn spec.pools.kubeletConfig.withContainerLogMaxSize

```ts
withContainerLogMaxSize(containerLogMaxSize)
```

"A quantity defines the maximum size of the container log file before it is rotated. For example: \"5Mi\" or \"256Ki\".\nDefault: 100Mi"

### fn spec.pools.kubeletConfig.withCpuCFSQuota

```ts
withCpuCFSQuota(cpuCFSQuota)
```

"CPUCFSQuota allows you to disable/enable CPU throttling for Pods."

### fn spec.pools.kubeletConfig.withCpuManagerPolicy

```ts
withCpuManagerPolicy(cpuManagerPolicy)
```

"CPUManagerPolicy allows to set alternative CPU management policies (default: none)."

### fn spec.pools.kubeletConfig.withEvictionMaxPodGracePeriod

```ts
withEvictionMaxPodGracePeriod(evictionMaxPodGracePeriod)
```

"EvictionMaxPodGracePeriod describes the maximum allowed grace period (in seconds) to use when terminating pods in response to a soft eviction threshold being met.\nDefault: 90"

### fn spec.pools.kubeletConfig.withEvictionPressureTransitionPeriod

```ts
withEvictionPressureTransitionPeriod(evictionPressureTransitionPeriod)
```

"EvictionPressureTransitionPeriod is the duration for which the kubelet has to wait before transitioning out of an eviction pressure condition.\nDefault: 4m0s"

### fn spec.pools.kubeletConfig.withFailSwapOn

```ts
withFailSwapOn(failSwapOn)
```

"FailSwapOn makes the Kubelet fail to start if swap is enabled on the node. (default true)."

### fn spec.pools.kubeletConfig.withFeatureGates

```ts
withFeatureGates(featureGates)
```

"FeatureGates contains information about enabled feature gates."

### fn spec.pools.kubeletConfig.withFeatureGatesMixin

```ts
withFeatureGatesMixin(featureGates)
```

"FeatureGates contains information about enabled feature gates."

**Note:** This function appends passed data to existing values

### fn spec.pools.kubeletConfig.withImageGCHighThresholdPercent

```ts
withImageGCHighThresholdPercent(imageGCHighThresholdPercent)
```

"ImageGCHighThresholdPercent describes the percent of the disk usage which triggers image garbage collection.\nDefault: 50"

### fn spec.pools.kubeletConfig.withImageGCLowThresholdPercent

```ts
withImageGCLowThresholdPercent(imageGCLowThresholdPercent)
```

"ImageGCLowThresholdPercent describes the percent of the disk to which garbage collection attempts to free.\nDefault: 40"

### fn spec.pools.kubeletConfig.withImageMaximumGCAge

```ts
withImageMaximumGCAge(imageMaximumGCAge)
```

"ImageMaximumGCAge is the maximum age of an unused image before it can be garbage collected.\nDefault: 0s"

### fn spec.pools.kubeletConfig.withImageMinimumGCAge

```ts
withImageMinimumGCAge(imageMinimumGCAge)
```

"ImageMinimumGCAge is the minimum age of an unused image before it can be garbage collected.\nDefault: 2m0s"

### fn spec.pools.kubeletConfig.withMaxParallelImagePulls

```ts
withMaxParallelImagePulls(maxParallelImagePulls)
```

"MaxParallelImagePulls describes the maximum number of image pulls in parallel. The value must be a positive number.\nThis field cannot be set if SerializeImagePulls (pull one image at a time) is set to true.\nSetting it to nil means no limit.\nDefault: nil"

### fn spec.pools.kubeletConfig.withMaxPods

```ts
withMaxPods(maxPods)
```

"MaxPods is the maximum number of Pods that are allowed by the Kubelet.\nDefault: 110"

### fn spec.pools.kubeletConfig.withPodPidsLimit

```ts
withPodPidsLimit(podPidsLimit)
```

"PodPIDsLimit is the maximum number of process IDs per pod allowed by the kubelet."

### fn spec.pools.kubeletConfig.withProtectKernelDefaults

```ts
withProtectKernelDefaults(protectKernelDefaults)
```

"ProtectKernelDefaults ensures that the kernel tunables are equal to the kubelet defaults.\nDefaults to true."

### fn spec.pools.kubeletConfig.withRegistryBurst

```ts
withRegistryBurst(registryBurst)
```

"RegistryBurst is the maximum size of bursty pulls, temporarily allows pulls to burst to this number,\nwhile still not exceeding registryPullQPS. The value must not be a negative number.\nOnly used if registryPullQPS is greater than 0.\nDefault: 10"

### fn spec.pools.kubeletConfig.withRegistryPullQPS

```ts
withRegistryPullQPS(registryPullQPS)
```

"RegistryPullQPS is the limit of registry pulls per second. The value must not be a negative number.\nSetting it to 0 means no limit.\nDefault: 5"

### fn spec.pools.kubeletConfig.withSeccompDefault

```ts
withSeccompDefault(seccompDefault)
```

"SeccompDefault enables the use of `RuntimeDefault` as the default seccomp profile for all workloads."

### fn spec.pools.kubeletConfig.withSerializeImagePulls

```ts
withSerializeImagePulls(serializeImagePulls)
```

"SerializeImagePulls describes whether the images are pulled one at a time.\nDefault: true"

### fn spec.pools.kubeletConfig.withStreamingConnectionIdleTimeout

```ts
withStreamingConnectionIdleTimeout(streamingConnectionIdleTimeout)
```

"StreamingConnectionIdleTimeout is the maximum time a streaming connection can be idle before the connection is automatically closed.\nThis field cannot be set lower than \"30s\" or greater than \"4h\".\nDefault: \"5m\"."

## obj spec.pools.kubeletConfig.evictionHard

"EvictionHard describes a set of eviction thresholds (e.g. memory.available<1Gi) that if met would trigger a Pod eviction.\nDefault:\n  memory.available:   \"100Mi/1Gi/5%\"\n  nodefs.available:   \"5%\"\n  nodefs.inodesFree:  \"5%\"\n  imagefs.available:  \"5%\"\n  imagefs.inodesFree: \"5%\

### fn spec.pools.kubeletConfig.evictionHard.withImageFSAvailable

```ts
withImageFSAvailable(imageFSAvailable)
```

"ImageFSAvailable is the threshold for the free disk space in the imagefs filesystem (docker images and container writable layers)."

### fn spec.pools.kubeletConfig.evictionHard.withImageFSInodesFree

```ts
withImageFSInodesFree(imageFSInodesFree)
```

"ImageFSInodesFree is the threshold for the available inodes in the imagefs filesystem."

### fn spec.pools.kubeletConfig.evictionHard.withMemoryAvailable

```ts
withMemoryAvailable(memoryAvailable)
```

"MemoryAvailable is the threshold for the free memory on the host server."

### fn spec.pools.kubeletConfig.evictionHard.withNodeFSAvailable

```ts
withNodeFSAvailable(nodeFSAvailable)
```

"NodeFSAvailable is the threshold for the free disk space in the nodefs filesystem (docker volumes, logs, etc)."

### fn spec.pools.kubeletConfig.evictionHard.withNodeFSInodesFree

```ts
withNodeFSInodesFree(nodeFSInodesFree)
```

"NodeFSInodesFree is the threshold for the available inodes in the nodefs filesystem."

## obj spec.pools.kubeletConfig.evictionMinimumReclaim

"EvictionMinimumReclaim configures the amount of resources below the configured eviction threshold that the kubelet attempts to reclaim whenever the kubelet observes resource pressure.\nDefault: 0 for each resource"

### fn spec.pools.kubeletConfig.evictionMinimumReclaim.withImageFSAvailable

```ts
withImageFSAvailable(imageFSAvailable)
```

"ImageFSAvailable is the threshold for the disk space reclaim in the imagefs filesystem (docker images and container writable layers)."

### fn spec.pools.kubeletConfig.evictionMinimumReclaim.withImageFSInodesFree

```ts
withImageFSInodesFree(imageFSInodesFree)
```

"ImageFSInodesFree is the threshold for the inodes reclaim in the imagefs filesystem."

### fn spec.pools.kubeletConfig.evictionMinimumReclaim.withMemoryAvailable

```ts
withMemoryAvailable(memoryAvailable)
```

"MemoryAvailable is the threshold for the memory reclaim on the host server."

### fn spec.pools.kubeletConfig.evictionMinimumReclaim.withNodeFSAvailable

```ts
withNodeFSAvailable(nodeFSAvailable)
```

"NodeFSAvailable is the threshold for the disk space reclaim in the nodefs filesystem (docker volumes, logs, etc)."

### fn spec.pools.kubeletConfig.evictionMinimumReclaim.withNodeFSInodesFree

```ts
withNodeFSInodesFree(nodeFSInodesFree)
```

"NodeFSInodesFree is the threshold for the inodes reclaim in the nodefs filesystem."

## obj spec.pools.kubeletConfig.evictionSoft

"EvictionSoft describes a set of eviction thresholds (e.g. memory.available<1.5Gi) that if met over a corresponding grace period would trigger a Pod eviction.\nDefault:\n  memory.available:   \"200Mi/1.5Gi/10%\"\n  nodefs.available:   \"10%\"\n  nodefs.inodesFree:  \"10%\"\n  imagefs.available:  \"10%\"\n  imagefs.inodesFree: \"10%\

### fn spec.pools.kubeletConfig.evictionSoft.withImageFSAvailable

```ts
withImageFSAvailable(imageFSAvailable)
```

"ImageFSAvailable is the threshold for the free disk space in the imagefs filesystem (docker images and container writable layers)."

### fn spec.pools.kubeletConfig.evictionSoft.withImageFSInodesFree

```ts
withImageFSInodesFree(imageFSInodesFree)
```

"ImageFSInodesFree is the threshold for the available inodes in the imagefs filesystem."

### fn spec.pools.kubeletConfig.evictionSoft.withMemoryAvailable

```ts
withMemoryAvailable(memoryAvailable)
```

"MemoryAvailable is the threshold for the free memory on the host server."

### fn spec.pools.kubeletConfig.evictionSoft.withNodeFSAvailable

```ts
withNodeFSAvailable(nodeFSAvailable)
```

"NodeFSAvailable is the threshold for the free disk space in the nodefs filesystem (docker volumes, logs, etc)."

### fn spec.pools.kubeletConfig.evictionSoft.withNodeFSInodesFree

```ts
withNodeFSInodesFree(nodeFSInodesFree)
```

"NodeFSInodesFree is the threshold for the available inodes in the nodefs filesystem."

## obj spec.pools.kubeletConfig.evictionSoftGracePeriod

"EvictionSoftGracePeriod describes a set of eviction grace periods (e.g. memory.available=1m30s) that correspond to how long a soft eviction threshold must hold before triggering a Pod eviction.\nDefault:\n  memory.available:   1m30s\n  nodefs.available:   1m30s\n  nodefs.inodesFree:  1m30s\n  imagefs.available:  1m30s\n  imagefs.inodesFree: 1m30s"

### fn spec.pools.kubeletConfig.evictionSoftGracePeriod.withImageFSAvailable

```ts
withImageFSAvailable(imageFSAvailable)
```

"ImageFSAvailable is the grace period for the ImageFSAvailable eviction threshold."

### fn spec.pools.kubeletConfig.evictionSoftGracePeriod.withImageFSInodesFree

```ts
withImageFSInodesFree(imageFSInodesFree)
```

"ImageFSInodesFree is the grace period for the ImageFSInodesFree eviction threshold."

### fn spec.pools.kubeletConfig.evictionSoftGracePeriod.withMemoryAvailable

```ts
withMemoryAvailable(memoryAvailable)
```

"MemoryAvailable is the grace period for the MemoryAvailable eviction threshold."

### fn spec.pools.kubeletConfig.evictionSoftGracePeriod.withNodeFSAvailable

```ts
withNodeFSAvailable(nodeFSAvailable)
```

"NodeFSAvailable is the grace period for the NodeFSAvailable eviction threshold."

### fn spec.pools.kubeletConfig.evictionSoftGracePeriod.withNodeFSInodesFree

```ts
withNodeFSInodesFree(nodeFSInodesFree)
```

"NodeFSInodesFree is the grace period for the NodeFSInodesFree eviction threshold."

## obj spec.pools.kubeletConfig.kubeReserved

"KubeReserved is the configuration for resources reserved for kubernetes node components (mainly kubelet and container runtime).\nWhen updating these values, be aware that cgroup resizes may not succeed on active worker nodes. Look for the NodeAllocatableEnforced event to determine if the configuration was applied.\nDefault: cpu=80m,memory=1Gi,pid=20k"

### fn spec.pools.kubeletConfig.kubeReserved.withCpu

```ts
withCpu(cpu)
```

"CPU is the reserved cpu."

### fn spec.pools.kubeletConfig.kubeReserved.withEphemeralStorage

```ts
withEphemeralStorage(ephemeralStorage)
```

"EphemeralStorage is the reserved ephemeral-storage."

### fn spec.pools.kubeletConfig.kubeReserved.withMemory

```ts
withMemory(memory)
```

"Memory is the reserved memory."

### fn spec.pools.kubeletConfig.kubeReserved.withPid

```ts
withPid(pid)
```

"PID is the reserved process-ids."

## obj spec.pools.kubeletConfig.memorySwap

"MemorySwap configures swap memory available to container workloads."

### fn spec.pools.kubeletConfig.memorySwap.withSwapBehavior

```ts
withSwapBehavior(swapBehavior)
```

"SwapBehavior configures swap memory available to container workloads. May be one of {\"NoSwap\", \"LimitedSwap\"}\ndefaults to: LimitedSwap"

## obj spec.pools.kubeletConfig.systemReserved

"SystemReserved is the configuration for resources reserved for system processes not managed by kubernetes (e.g. journald).\nWhen updating these values, be aware that cgroup resizes may not succeed on active worker nodes. Look for the NodeAllocatableEnforced event to determine if the configuration was applied.\n\nDeprecated: Separately configuring resource reservations for system processes is deprecated in Gardener and will be forbidden starting from Kubernetes 1.31.\nPlease merge existing resource reservations into the kubeReserved field."

### fn spec.pools.kubeletConfig.systemReserved.withCpu

```ts
withCpu(cpu)
```

"CPU is the reserved cpu."

### fn spec.pools.kubeletConfig.systemReserved.withEphemeralStorage

```ts
withEphemeralStorage(ephemeralStorage)
```

"EphemeralStorage is the reserved ephemeral-storage."

### fn spec.pools.kubeletConfig.systemReserved.withMemory

```ts
withMemory(memory)
```

"Memory is the reserved memory."

### fn spec.pools.kubeletConfig.systemReserved.withPid

```ts
withPid(pid)
```

"PID is the reserved process-ids."

## obj spec.pools.machineControllerManager

"MachineControllerManagerSettings contains configurations for different worker-pools. Eg. MachineDrainTimeout, MachineHealthTimeout."

### fn spec.pools.machineControllerManager.withDisableHealthTimeout

```ts
withDisableHealthTimeout(disableHealthTimeout)
```

"DisableHealthTimeout if set to true, health timeout will be ignored. Leading to machine never being declared failed.\nThis is intended to be used only for in-place updates."

### fn spec.pools.machineControllerManager.withInPlaceUpdateTimeout

```ts
withInPlaceUpdateTimeout(inPlaceUpdateTimeout)
```

"MachineInPlaceUpdateTimeout is the timeout after which in-place update is declared failed."

### fn spec.pools.machineControllerManager.withMachineCreationTimeout

```ts
withMachineCreationTimeout(machineCreationTimeout)
```

"MachineCreationTimeout is the period after which creation of the machine is declared failed."

### fn spec.pools.machineControllerManager.withMachineDrainTimeout

```ts
withMachineDrainTimeout(machineDrainTimeout)
```

"MachineDrainTimeout is the period after which machine is forcefully deleted."

### fn spec.pools.machineControllerManager.withMachineHealthTimeout

```ts
withMachineHealthTimeout(machineHealthTimeout)
```

"MachineHealthTimeout is the period after which machine is declared failed."

### fn spec.pools.machineControllerManager.withMaxEvictRetries

```ts
withMaxEvictRetries(maxEvictRetries)
```

"MaxEvictRetries are the number of eviction retries on a pod after which drain is declared failed, and forceful deletion is triggered."

### fn spec.pools.machineControllerManager.withNodeConditions

```ts
withNodeConditions(nodeConditions)
```

"NodeConditions are the set of conditions if set to true for the period of MachineHealthTimeout, machine will be declared failed."

### fn spec.pools.machineControllerManager.withNodeConditionsMixin

```ts
withNodeConditionsMixin(nodeConditions)
```

"NodeConditions are the set of conditions if set to true for the period of MachineHealthTimeout, machine will be declared failed."

**Note:** This function appends passed data to existing values

## obj spec.pools.machineImage

"MachineImage contains logical information about the name and the version of the machie image that\nshould be used. The logical information must be mapped to the provider-specific information (e.g.,\nAMIs, ...) by the provider itself."

### fn spec.pools.machineImage.withName

```ts
withName(name)
```

"Name is the logical name of the machine image."

### fn spec.pools.machineImage.withVersion

```ts
withVersion(version)
```

"Version is the version of the machine image."

## obj spec.pools.nodeTemplate

"NodeTemplate contains resource information of the machine which is used by Cluster Autoscaler to generate nodeTemplate during scaling a nodeGroup"

### fn spec.pools.nodeTemplate.withCapacity

```ts
withCapacity(capacity)
```

"Capacity represents the expected Node capacity."

### fn spec.pools.nodeTemplate.withCapacityMixin

```ts
withCapacityMixin(capacity)
```

"Capacity represents the expected Node capacity."

**Note:** This function appends passed data to existing values

### fn spec.pools.nodeTemplate.withVirtualCapacity

```ts
withVirtualCapacity(virtualCapacity)
```

"VirtualCapacity represents the expected Node 'virtual' capacity ie comprising virtual extended resources."

### fn spec.pools.nodeTemplate.withVirtualCapacityMixin

```ts
withVirtualCapacityMixin(virtualCapacity)
```

"VirtualCapacity represents the expected Node 'virtual' capacity ie comprising virtual extended resources."

**Note:** This function appends passed data to existing values

## obj spec.pools.taints

"Taints is a list of taints for all the `Node` objects in this worker pool."

### fn spec.pools.taints.withEffect

```ts
withEffect(effect)
```

"Required. The effect of the taint on pods\nthat do not tolerate the taint.\nValid effects are NoSchedule, PreferNoSchedule and NoExecute."

### fn spec.pools.taints.withKey

```ts
withKey(key)
```

"Required. The taint key to be applied to a node."

### fn spec.pools.taints.withTimeAdded

```ts
withTimeAdded(timeAdded)
```

"TimeAdded represents the time at which the taint was added."

### fn spec.pools.taints.withValue

```ts
withValue(value)
```

"The taint value corresponding to the taint key."

## obj spec.pools.userDataSecretRef

"UserDataSecretRef references a Secret and a data key containing the data that is sent to the provider's APIs when\na new machine/VM that is part of this worker pool shall be spawned."

### fn spec.pools.userDataSecretRef.withKey

```ts
withKey(key)
```

"The key of the secret to select from.  Must be a valid secret key."

### fn spec.pools.userDataSecretRef.withName

```ts
withName(name)
```

"Name of the referent.\nThis field is effectively required, but due to backwards compatibility is\nallowed to be empty. Instances of this type with an empty value here are\nalmost certainly wrong.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

### fn spec.pools.userDataSecretRef.withOptional

```ts
withOptional(optional)
```

"Specify whether the Secret or its key must be defined"

## obj spec.pools.volume

"Volume contains information about the root disks that should be used for this worker pool."

### fn spec.pools.volume.withEncrypted

```ts
withEncrypted(encrypted)
```

"Encrypted determines if the volume should be encrypted."

### fn spec.pools.volume.withName

```ts
withName(name)
```

"Name of the volume to make it referenceable."

### fn spec.pools.volume.withSize

```ts
withSize(size)
```

"Size is the of the root volume."

### fn spec.pools.volume.withType

```ts
withType(type)
```

"Type is the type of the volume."

## obj spec.secretRef

"SecretRef is a reference to a secret that contains the cloud provider specific credentials."

### fn spec.secretRef.withName

```ts
withName(name)
```

"name is unique within a namespace to reference a secret resource."

### fn spec.secretRef.withNamespace

```ts
withNamespace(namespace)
```

"namespace defines the space within which the secret name must be unique."