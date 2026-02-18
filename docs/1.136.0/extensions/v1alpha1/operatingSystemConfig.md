---
permalink: /1.136.0/extensions/v1alpha1/operatingSystemConfig/
---

# extensions.v1alpha1.operatingSystemConfig

"OperatingSystemConfig is a specification for a OperatingSystemConfig resource"

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
  * [`fn withFiles(files)`](#fn-specwithfiles)
  * [`fn withFilesMixin(files)`](#fn-specwithfilesmixin)
  * [`fn withProviderConfig(providerConfig)`](#fn-specwithproviderconfig)
  * [`fn withProviderConfigMixin(providerConfig)`](#fn-specwithproviderconfigmixin)
  * [`fn withPurpose(purpose)`](#fn-specwithpurpose)
  * [`fn withType(type)`](#fn-specwithtype)
  * [`fn withUnits(units)`](#fn-specwithunits)
  * [`fn withUnitsMixin(units)`](#fn-specwithunitsmixin)
  * [`obj spec.criConfig`](#obj-speccriconfig)
    * [`fn withCgroupDriver(cgroupDriver)`](#fn-speccriconfigwithcgroupdriver)
    * [`fn withName(name)`](#fn-speccriconfigwithname)
    * [`obj spec.criConfig.containerd`](#obj-speccriconfigcontainerd)
      * [`fn withPlugins(plugins)`](#fn-speccriconfigcontainerdwithplugins)
      * [`fn withPluginsMixin(plugins)`](#fn-speccriconfigcontainerdwithpluginsmixin)
      * [`fn withRegistries(registries)`](#fn-speccriconfigcontainerdwithregistries)
      * [`fn withRegistriesMixin(registries)`](#fn-speccriconfigcontainerdwithregistriesmixin)
      * [`fn withSandboxImage(sandboxImage)`](#fn-speccriconfigcontainerdwithsandboximage)
      * [`obj spec.criConfig.containerd.plugins`](#obj-speccriconfigcontainerdplugins)
        * [`fn withOp(op)`](#fn-speccriconfigcontainerdpluginswithop)
        * [`fn withPath(path)`](#fn-speccriconfigcontainerdpluginswithpath)
        * [`fn withPathMixin(path)`](#fn-speccriconfigcontainerdpluginswithpathmixin)
        * [`fn withValues(values)`](#fn-speccriconfigcontainerdpluginswithvalues)
      * [`obj spec.criConfig.containerd.registries`](#obj-speccriconfigcontainerdregistries)
        * [`fn withHosts(hosts)`](#fn-speccriconfigcontainerdregistrieswithhosts)
        * [`fn withHostsMixin(hosts)`](#fn-speccriconfigcontainerdregistrieswithhostsmixin)
        * [`fn withReadinessProbe(readinessProbe)`](#fn-speccriconfigcontainerdregistrieswithreadinessprobe)
        * [`fn withServer(server)`](#fn-speccriconfigcontainerdregistrieswithserver)
        * [`fn withUpstream(upstream)`](#fn-speccriconfigcontainerdregistrieswithupstream)
        * [`obj spec.criConfig.containerd.registries.hosts`](#obj-speccriconfigcontainerdregistrieshosts)
          * [`fn withCaCerts(caCerts)`](#fn-speccriconfigcontainerdregistrieshostswithcacerts)
          * [`fn withCaCertsMixin(caCerts)`](#fn-speccriconfigcontainerdregistrieshostswithcacertsmixin)
          * [`fn withCapabilities(capabilities)`](#fn-speccriconfigcontainerdregistrieshostswithcapabilities)
          * [`fn withCapabilitiesMixin(capabilities)`](#fn-speccriconfigcontainerdregistrieshostswithcapabilitiesmixin)
          * [`fn withOverridePath(overridePath)`](#fn-speccriconfigcontainerdregistrieshostswithoverridepath)
          * [`fn withUrl(url)`](#fn-speccriconfigcontainerdregistrieshostswithurl)
  * [`obj spec.files`](#obj-specfiles)
    * [`fn withPath(path)`](#fn-specfileswithpath)
    * [`fn withPermissions(permissions)`](#fn-specfileswithpermissions)
    * [`obj spec.files.content`](#obj-specfilescontent)
      * [`fn withTransmitUnencoded(transmitUnencoded)`](#fn-specfilescontentwithtransmitunencoded)
      * [`obj spec.files.content.imageRef`](#obj-specfilescontentimageref)
        * [`fn withFilePathInImage(filePathInImage)`](#fn-specfilescontentimagerefwithfilepathinimage)
        * [`fn withImage(image)`](#fn-specfilescontentimagerefwithimage)
      * [`obj spec.files.content.inline`](#obj-specfilescontentinline)
        * [`fn withData(data)`](#fn-specfilescontentinlinewithdata)
        * [`fn withEncoding(encoding)`](#fn-specfilescontentinlinewithencoding)
      * [`obj spec.files.content.secretRef`](#obj-specfilescontentsecretref)
        * [`fn withDataKey(dataKey)`](#fn-specfilescontentsecretrefwithdatakey)
        * [`fn withName(name)`](#fn-specfilescontentsecretrefwithname)
  * [`obj spec.inPlaceUpdates`](#obj-specinplaceupdates)
    * [`fn withKubelet(kubelet)`](#fn-specinplaceupdateswithkubelet)
    * [`fn withOperatingSystemVersion(operatingSystemVersion)`](#fn-specinplaceupdateswithoperatingsystemversion)
    * [`obj spec.inPlaceUpdates.credentialsRotation`](#obj-specinplaceupdatescredentialsrotation)
      * [`obj spec.inPlaceUpdates.credentialsRotation.certificateAuthorities`](#obj-specinplaceupdatescredentialsrotationcertificateauthorities)
        * [`fn withLastInitiationTime(lastInitiationTime)`](#fn-specinplaceupdatescredentialsrotationcertificateauthoritieswithlastinitiationtime)
      * [`obj spec.inPlaceUpdates.credentialsRotation.serviceAccountKey`](#obj-specinplaceupdatescredentialsrotationserviceaccountkey)
        * [`fn withLastInitiationTime(lastInitiationTime)`](#fn-specinplaceupdatescredentialsrotationserviceaccountkeywithlastinitiationtime)
  * [`obj spec.units`](#obj-specunits)
    * [`fn withCommand(command)`](#fn-specunitswithcommand)
    * [`fn withContent(content)`](#fn-specunitswithcontent)
    * [`fn withDropIns(dropIns)`](#fn-specunitswithdropins)
    * [`fn withDropInsMixin(dropIns)`](#fn-specunitswithdropinsmixin)
    * [`fn withEnable(enable)`](#fn-specunitswithenable)
    * [`fn withFilePaths(filePaths)`](#fn-specunitswithfilepaths)
    * [`fn withFilePathsMixin(filePaths)`](#fn-specunitswithfilepathsmixin)
    * [`fn withName(name)`](#fn-specunitswithname)
    * [`obj spec.units.dropIns`](#obj-specunitsdropins)
      * [`fn withContent(content)`](#fn-specunitsdropinswithcontent)
      * [`fn withName(name)`](#fn-specunitsdropinswithname)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of OperatingSystemConfig

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

"Specification of the OperatingSystemConfig.\nIf the object's deletion timestamp is set, this field is immutable."

### fn spec.withClass

```ts
withClass(class)
```

"Class holds the extension class used to control the responsibility for multiple provider extensions."

### fn spec.withFiles

```ts
withFiles(files)
```

"Files is a list of files that should get written to the host's file system."

### fn spec.withFilesMixin

```ts
withFilesMixin(files)
```

"Files is a list of files that should get written to the host's file system."

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

### fn spec.withPurpose

```ts
withPurpose(purpose)
```

"Purpose describes how the result of this OperatingSystemConfig is used by Gardener. Either it\ngets sent to the `Worker` extension controller to bootstrap a VM, or it is downloaded by the\ngardener-node-agent already running on a bootstrapped VM.\nThis field is immutable."

### fn spec.withType

```ts
withType(type)
```

"Type contains the instance of the resource's kind."

### fn spec.withUnits

```ts
withUnits(units)
```

"Units is a list of unit for the operating system configuration (usually, a systemd unit)."

### fn spec.withUnitsMixin

```ts
withUnitsMixin(units)
```

"Units is a list of unit for the operating system configuration (usually, a systemd unit)."

**Note:** This function appends passed data to existing values

## obj spec.criConfig

"CRI config is a structure contains configurations of the CRI library"

### fn spec.criConfig.withCgroupDriver

```ts
withCgroupDriver(cgroupDriver)
```

"CgroupDriver configures the CRI's cgroup driver. Supported values are `cgroupfs` or `systemd`."

### fn spec.criConfig.withName

```ts
withName(name)
```

"Name is a mandatory string containing the name of the CRI library. Supported values are `containerd`."

## obj spec.criConfig.containerd

"ContainerdConfig is the containerd configuration.\nOnly to be set for OperatingSystemConfigs with purpose 'reconcile'."

### fn spec.criConfig.containerd.withPlugins

```ts
withPlugins(plugins)
```

"Plugins configures the plugins section in containerd's config.toml."

### fn spec.criConfig.containerd.withPluginsMixin

```ts
withPluginsMixin(plugins)
```

"Plugins configures the plugins section in containerd's config.toml."

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.withRegistries

```ts
withRegistries(registries)
```

"Registries configures the registry hosts for containerd."

### fn spec.criConfig.containerd.withRegistriesMixin

```ts
withRegistriesMixin(registries)
```

"Registries configures the registry hosts for containerd."

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.withSandboxImage

```ts
withSandboxImage(sandboxImage)
```

"SandboxImage configures the sandbox image for containerd."

## obj spec.criConfig.containerd.plugins

"Plugins configures the plugins section in containerd's config.toml."

### fn spec.criConfig.containerd.plugins.withOp

```ts
withOp(op)
```

"Op is the operation for the given path. Possible values are 'add' and 'remove', defaults to 'add'."

### fn spec.criConfig.containerd.plugins.withPath

```ts
withPath(path)
```

"Path is a list of elements that construct the path in the plugins section."

### fn spec.criConfig.containerd.plugins.withPathMixin

```ts
withPathMixin(path)
```

"Path is a list of elements that construct the path in the plugins section."

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.plugins.withValues

```ts
withValues(values)
```

"Values are the values configured at the given path. If defined, it is expected as json format:\n- A given json object will be put to the given path.\n- If not configured, only the table entry to be created."

## obj spec.criConfig.containerd.registries

"Registries configures the registry hosts for containerd."

### fn spec.criConfig.containerd.registries.withHosts

```ts
withHosts(hosts)
```

"Hosts are the registry hosts.\nIt corresponds to the host fields in the `hosts.toml` file, see https://github.com/containerd/containerd/blob/c51463010e0682f76dfdc10edc095e6596e2764b/docs/hosts.md#host-fields-in-the-toml-table-format for more information."

### fn spec.criConfig.containerd.registries.withHostsMixin

```ts
withHostsMixin(hosts)
```

"Hosts are the registry hosts.\nIt corresponds to the host fields in the `hosts.toml` file, see https://github.com/containerd/containerd/blob/c51463010e0682f76dfdc10edc095e6596e2764b/docs/hosts.md#host-fields-in-the-toml-table-format for more information."

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.registries.withReadinessProbe

```ts
withReadinessProbe(readinessProbe)
```

"ReadinessProbe determines if host registry endpoints should be probed before they are added to the containerd config."

### fn spec.criConfig.containerd.registries.withServer

```ts
withServer(server)
```

"Server is the URL to registry server of this upstream.\nIt corresponds to the server field in the `hosts.toml` file, see https://github.com/containerd/containerd/blob/c51463010e0682f76dfdc10edc095e6596e2764b/docs/hosts.md#server-field for more information."

### fn spec.criConfig.containerd.registries.withUpstream

```ts
withUpstream(upstream)
```

"Upstream is the upstream name of the registry."

## obj spec.criConfig.containerd.registries.hosts

"Hosts are the registry hosts.\nIt corresponds to the host fields in the `hosts.toml` file, see https://github.com/containerd/containerd/blob/c51463010e0682f76dfdc10edc095e6596e2764b/docs/hosts.md#host-fields-in-the-toml-table-format for more information."

### fn spec.criConfig.containerd.registries.hosts.withCaCerts

```ts
withCaCerts(caCerts)
```

"CACerts are paths to public key certificates used for TLS."

### fn spec.criConfig.containerd.registries.hosts.withCaCertsMixin

```ts
withCaCertsMixin(caCerts)
```

"CACerts are paths to public key certificates used for TLS."

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.registries.hosts.withCapabilities

```ts
withCapabilities(capabilities)
```

"Capabilities determine what operations a host is\ncapable of performing. Defaults to\n - pull\n - resolve"

### fn spec.criConfig.containerd.registries.hosts.withCapabilitiesMixin

```ts
withCapabilitiesMixin(capabilities)
```

"Capabilities determine what operations a host is\ncapable of performing. Defaults to\n - pull\n - resolve"

**Note:** This function appends passed data to existing values

### fn spec.criConfig.containerd.registries.hosts.withOverridePath

```ts
withOverridePath(overridePath)
```

"OverridePath sets the 'override_path' field to allow defining the API endpoint in the URL.\nSee https://github.com/containerd/containerd/blob/cef8ce2ecb572bc8026323c0c3dfad9953b952f6/docs/hosts.md?override_path#override_path-field for more information."

### fn spec.criConfig.containerd.registries.hosts.withUrl

```ts
withUrl(url)
```

"URL is the endpoint address of the registry mirror."

## obj spec.files

"Files is a list of files that should get written to the host's file system."

### fn spec.files.withPath

```ts
withPath(path)
```

"Path is the path of the file system where the file should get written to."

### fn spec.files.withPermissions

```ts
withPermissions(permissions)
```

"Permissions describes with which permissions the file should get written to the file system.\nIf no permissions are set, the operating system's defaults are used."

## obj spec.files.content

"Content describe the file's content."

### fn spec.files.content.withTransmitUnencoded

```ts
withTransmitUnencoded(transmitUnencoded)
```

"TransmitUnencoded set to true will ensure that the os-extension does not encode the file content when sent to the node.\nThis for example can be used to manipulate the clear-text content before it reaches the node."

## obj spec.files.content.imageRef

"ImageRef describes a container image which contains a file."

### fn spec.files.content.imageRef.withFilePathInImage

```ts
withFilePathInImage(filePathInImage)
```

"FilePathInImage contains the path in the image to the file that should be extracted."

### fn spec.files.content.imageRef.withImage

```ts
withImage(image)
```

"Image contains the container image repository with tag."

## obj spec.files.content.inline

"Inline is a struct that contains information about the inlined data."

### fn spec.files.content.inline.withData

```ts
withData(data)
```

"Data is the file's data."

### fn spec.files.content.inline.withEncoding

```ts
withEncoding(encoding)
```

"Encoding is the file's encoding (e.g. base64)."

## obj spec.files.content.secretRef

"SecretRef is a struct that contains information about the referenced secret."

### fn spec.files.content.secretRef.withDataKey

```ts
withDataKey(dataKey)
```

"DataKey is the key in the secret's `.data` field that should be read."

### fn spec.files.content.secretRef.withName

```ts
withName(name)
```

"Name is the name of the secret."

## obj spec.inPlaceUpdates

"InPlaceUpdates contains the configuration for in-place updates."

### fn spec.inPlaceUpdates.withKubelet

```ts
withKubelet(kubelet)
```

"KubeletVersion is the version of the kubelet."

### fn spec.inPlaceUpdates.withOperatingSystemVersion

```ts
withOperatingSystemVersion(operatingSystemVersion)
```

"OperatingSystemVersion is the version of the operating system."

## obj spec.inPlaceUpdates.credentialsRotation

"CredentialsRotation is a structure containing information about the last initiation time of the certificate authority and service account key rotation."

## obj spec.inPlaceUpdates.credentialsRotation.certificateAuthorities

"CertificateAuthorities contains information about the certificate authority credential rotation."

### fn spec.inPlaceUpdates.credentialsRotation.certificateAuthorities.withLastInitiationTime

```ts
withLastInitiationTime(lastInitiationTime)
```

"LastInitiationTime is the most recent time when the certificate authority credential rotation was initiated."

## obj spec.inPlaceUpdates.credentialsRotation.serviceAccountKey

"ServiceAccountKey contains information about the service account key credential rotation."

### fn spec.inPlaceUpdates.credentialsRotation.serviceAccountKey.withLastInitiationTime

```ts
withLastInitiationTime(lastInitiationTime)
```

"LastInitiationTime is the most recent time when the service account key credential rotation was initiated."

## obj spec.units

"Units is a list of unit for the operating system configuration (usually, a systemd unit)."

### fn spec.units.withCommand

```ts
withCommand(command)
```

"Command is the unit's command."

### fn spec.units.withContent

```ts
withContent(content)
```

"Content is the unit's content."

### fn spec.units.withDropIns

```ts
withDropIns(dropIns)
```

"DropIns is a list of drop-ins for this unit."

### fn spec.units.withDropInsMixin

```ts
withDropInsMixin(dropIns)
```

"DropIns is a list of drop-ins for this unit."

**Note:** This function appends passed data to existing values

### fn spec.units.withEnable

```ts
withEnable(enable)
```

"Enable describes whether the unit is enabled or not."

### fn spec.units.withFilePaths

```ts
withFilePaths(filePaths)
```

"FilePaths is a list of files the unit depends on. If any file changes a restart of the dependent unit will be\ntriggered. For each FilePath there must exist a File with matching Path in OperatingSystemConfig.Spec.Files."

### fn spec.units.withFilePathsMixin

```ts
withFilePathsMixin(filePaths)
```

"FilePaths is a list of files the unit depends on. If any file changes a restart of the dependent unit will be\ntriggered. For each FilePath there must exist a File with matching Path in OperatingSystemConfig.Spec.Files."

**Note:** This function appends passed data to existing values

### fn spec.units.withName

```ts
withName(name)
```

"Name is the name of a unit."

## obj spec.units.dropIns

"DropIns is a list of drop-ins for this unit."

### fn spec.units.dropIns.withContent

```ts
withContent(content)
```

"Content is the content of the drop-in."

### fn spec.units.dropIns.withName

```ts
withName(name)
```

"Name is the name of the drop-in."