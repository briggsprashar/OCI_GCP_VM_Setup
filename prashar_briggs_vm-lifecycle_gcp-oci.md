# OCI & GCP basic Virtual Machine (VM) setup 
*Created from a .edu account and by selecting the bare minimum resources/options for least billing.*

## **Video Walkthrough**

### OCI - Oracle Cloud Infastructure

<div>
  <a style="float: left;">
  Creating a Virtual Machine on Oracle Cloud Infrastructure ☁️
  </a>
  <a href="https://www.loom.com/share/247f1b94e7df45fabbe65d92f6247c09" style="float: left;" style="float: right;">
  <img style="max-width:100px;" src="https://cdn.loom.com/sessions/thumbnails/247f1b94e7df45fabbe65d92f6247c09-1d8a737df9869677-full-play.gif" />
  </a>
  <div style="clear: both;"></div>

### GCP - Google Cloud Platform

<div>
  <a style="float: left;">
  Creating a Virtual Machine on Google Cloud ☁️
  </a>
  <a href="https://www.loom.com/share/0c5531756ef945c08d0fd9cecb2ffd26" style="float: left;" style="float: right;">
  <img style="max-width:100px;" src="https://cdn.loom.com/sessions/thumbnails/247f1b94e7df45fabbe65d92f6247c09-1d8a737df9869677-full-play.gif" />
  </a>
  <div style="clear: both;"></div>

<br />
<br />
<details open>
  <summary>Prerequisites</summary>  
<br />

- Access to GCP and OCI cloud consoles
- $ Credits (and educational affiliation to get credits)  
- Basic and least-expensive/free-tier/smallest VM configurations
- Compliance to all healthcare related regulations, especially with PHI/PII data
</details>

## **VM configuration and creation steps**

## Oracle Cloud Infrastructure (OCI)

<details>
  <summary>Configuration</summary>  
<br />

1. **Compartment**: `briggsp`  
3. **Shape**: `VM.Standard.E2.1.Micro`
4. **Image**: `Ubuntu`  
5. **Public IP**: `Ephemeral IPv4`
2. **Networking**: `Virtual Cloud Network (VCN) with default security configuration`
6. **Boot Volume**: `Default minimal`
</details>

<details>
  <summary>VM creation in Images</summary>  
<br />



Steps 1 to 19 (Click on an image to view the full size image)

| 1 ACCOUNT [![Account](OCI/1-acct-provisioned.png)](OCI/1-acct-provisioned.png) | 2 Navigation [![Navigation](OCI/2-navigation-options.png)](OCI/2-navigation-options.png) |
|--------------------------------------------------|--------------------------------------------------|
| 3 Create INSTANCE [![Instance](OCI/3-instance-page.png)](OCI/3-instance-page.png) | 4 BASIC INFO [![Basic Info](OCI/4-basic-info.png)](OCI/4-basic-info.png) |
| 5 Select IMAGE [![Image](OCI/5-image.png)](OCI/5-image.png) | 6 UBUNTU [![Ubuntu](OCI/5.1-images.png)](OCI/5.1-images.png) |
| 7 Image Name [![Image name](OCI/5.2-images.png)](OCI/5.2-images.png) | 8 Select SHAPE [![Shape](OCI/6-shape.png)](OCI/6-shape.png) |
| 9 All Shapes [![All Shapes](OCI/6.1-shape.png)](OCI/6.1-shape.png) | 10 Shape Name [![Shape name](OCI/6.2-shape.png)](OCI/6.2-shape.png) |
| 11 SECURITY [![Security](OCI/7-security.png)](OCI/7-security.png) | 12 NETWORKING [![Network](OCI/8-networking.png)](OCI/8-networking.png) |
| 13 SSH [![SSH](OCI/8.1-networking.png)](OCI/8.1-networking.png) | 14 BOOT Volume [![Boot Volume](OCI/9-boot-volume.png)](OCI/9-boot-volume.png) |
| 15 REVIEW [![Review](OCI/10-review.png)](OCI/10-review.png) | 16 Work Requests [![Work requests](OCI/11-work-requests.png)](OCI/11-work-requests.png) |
| 17 Instances List [![Instances](OCI/12-terminate.png)](OCI/12-terminate.png) | 18 Navigation [![Navigation](OCI/13-navbar-infrastructure.png)](OCI/13-navbar-infrastructure.png) |
| 19 DASHBOARD [![Dashboard](OCI/14-dashboard.png)](OCI/14-dashboard.png) | 

</details>

<details>
  <summary>OCI VM lifecycle management</summary>  
<br />

| 1 VM-Provisioning [![VM-Provisioning](OCI1/1ociprovisioning.png)](OCI1/1ociprovisioning.png) | 2 VM Created [![VM Created](OCI1/2ocirunningsucceeded.png)](OCI1/2ocirunningsucceeded.png) |
|--------------------------------------------------|--------------------------------------------------|
| 3 VM Running [![VM Running](OCI1/3ociinstancesrunning.png)](OCI1/3ociinstancesrunning.png) | 4 VM Stopped [![VM Stopped](OCI1/5stopped.png)](OCI1/5stopped.png)) |
| 5 VM Terminating [![VM Terminating](OCI1/6ociterminating.png)](OCI1/6ociterminating.png) | 7 VM Terminated [![VM Terminated](OCI1/8oiterminatedinstance.png)](OCI1/8oiterminatedinstance.png) |
| 7 OCI Resources [![OCI Resources](OCI1/9ocIresourceexplorere.png)](OCI1/9ocIresourceexplorere.png) | 
</details>


---

## Google Cloud Platform (GCP) 

<details>
  <summary>Configuration</summary>  
<br />

1. Navigate to: **Console → Compute Engine → Create Instance**  
2. **Region/Zone**: `us-east (Columbus)` / `Default`
3. **Machine Type**: `(General Purpose) e2-micro` (2 vCPU, 1 core, 1 GB memory)  
4. **Image**: `Ubuntu LTS`  
5. **Boot Disk**: `Default minimal`  
6. **Network**: `Default Ephemeral IPv4`
7. **CostMonthly Estimate**: `$7.11` with variable cost for data protection with snapshot schedule

</details>

<details>
  <summary>VM creation in Images</summary>  
<br />

Steps 1 to 14 (Click on an image to view the full size image)

| 1 ACCOUNT [![Account](GCP/1_ACCOUNT.png)](GCP/1_ACCOUNT.png) | 2 VM Instance [![VM Instance](GCP/2_VM-Instances.png)](GCP/2_VM-Instances.png) |
|--------------------------------------------------|--------------------------------------------------|
| 3 Create INSTANCE [![Create Instance](GCP/3_Create-Instance.png)](GCP/3_Create-Instance.png) | 4 Machine Configuration [![Machine Configuration](GCP/4_Machine-Configuration.png)](GCP/4_Machine-Configuration.png) |
| 5 Cost Optimized View [![Image](GCP/5_Cost-Optimized.png)](GCP/5_Cost-Optimized.png) | 6 OS STORAGE [![OS Storage](GCP/6_OS-Storage.png)](GCP/6_OS-Storage.png) |
| 7 DATA PROTECTION [![Data Protection](GCP/7_Data-Protection.png)](GCP/7_Data-Protection.png) | 8 NETWORKING [![NETWORKING](GCP/8_Networking.png)](GCP/8_Networking.png) |
| 9 OBSERVABILITY [![Observability](GCP/9_Observability.png)](GCP/9_Observability.png) | 10 SECURITY [![Security](GCP/10_Security.png)](GCP/10_Security.png) |
| 11 Advanced [![Advanced](GCP/11_Advanced.png)](GCP/11_Advanced.png) | 12 VM Created [![VM Created](GCP/12_VM-created.png)](GCP/12_VM-created.png) |
| 13 OBSERVABILITY [![Observability](GCP/13_Observability.png)](GCP/13_Observability.png) | 14 OVERVIEW [![Overview](GCP/14_Overview.png)](GCP/14_Overview.png) |

</details>

<details>
  <summary>GCP VM lifecycle management</summary>  
<br />

| 1 VM Running [![VM Running](GCP1/2gcprunning.png)](GCP1/2gcprunning.png) | 2 VM Stopped [![VM Stopped](GCP1/4gcpstopped.png)](GCP1/4gcpstopped.png) |
|--------------------------------------------------|--------------------------------------------------|
| 3 VM Actions [![VM Actions](GCP1/5gcpdelete.png)](GCP1/5gcpdelete.png) | 4 VM Deleted [![VM Deleted](GCP1/6gcpdeleted.png)](GCP1/6gcpdeleted.png) |
| 5 Operations List  [![Operations List](GCP1/7gcpoperationfinished.png)](GCP1/7gcpoperationfinished.png) | 6 Overview [![Overview](GCP1/8gcpoverview.png)](GCP1/8gcpoverview.png) |

</details>

## Reflections

<details>
  <summary>Key Similarities in VM setup</summary>  
<br />

- Education credits for free usage
- Custom VM configuration
- VM Creation steps similar in nature and flow
- Region, Zone and VM specification setup
- Customization 
- Differentiate between ephemeral and static IP's
- Offer private default private networks with internet access
- Global datacenter presence supporting multi-region deployments
- Auto scaling capabilities
</details>

<details>
  <summary>Key Differences in VM setup</summary>  
<br />

- OCI has a technical VM setup than GCP.
- OCI provides for creating variables like subnet if not auto-populated; GCP does not offer this, suggesting these variables get resolved automatically in the backend
- OCI containers are tenancy-name/root; GCP container is autogenerated in the backend
- GCP offers a cost estimate and configuration snapshot throughout the VM creation process; OCI does not
- GCP is more user friendly with a better UI and UX compared to OCI
- GCP overview and dashboard view, both very comprehensive
- GCP has a configurable observability feature offering resources usage from various angles
- SSH keys and configuration is auto generated in GCP. In OCI it is manually done with SSH kep downloaded manually
- GCP has more OS variety than GCP
</details>

## Discussion

OCI appears to provide lower cost VM instances (reduces costs). GCP offers a wider global reach and strong analytics capabilities and other bells and whistles for AI capabilities. GCP has a better UI and UX. GCP has more analytics capabilities. GC seems to offer more customization and scalability options. It is also easier to migrate VM instances into GCP from other platforms. GCP seems more user friendly. Overall, between OCI and GCP, GCP seems a better option with the AI and bigdata capabilities and opportunities. OCI seems to be a no frills option for cost reduction and for needs that are not that variable in classic industries.  

