# OCI & GCP basic Virtual Machine setup 
*Created from a .edu account and selecting the bare minimum resources/options for least billing.*

## Video Walkthrough 

#### OCI - Oracle Cloud Infastructure

<div>
    <a href="https://www.loom.com/share/247f1b94e7df45fabbe65d92f6247c09">
      <p>Creating a Virtual Machine on Oracle Cloud Infrastructure ☁️ - Watch Video</p>
    </a>
    <a href="https://www.loom.com/share/247f1b94e7df45fabbe65d92f6247c09">
      <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/247f1b94e7df45fabbe65d92f6247c09-1d8a737df9869677-full-play.gif">
    </a>
  </div>

#### GCP - Google Cloud Platform

<div>
    <a href="https://www.loom.com/share/0c5531756ef945c08d0fd9cecb2ffd26">
      <p>Creating a Virtual Machine on Google Cloud ☁️ - Watch Video</p>
    </a>
    <a href="https://www.loom.com/share/0c5531756ef945c08d0fd9cecb2ffd26">
      <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/0c5531756ef945c08d0fd9cecb2ffd26-90ea5b3616f74890-full-play.gif">
    </a>
  </div>

## Prerequisites
- Access to GCP and OCI cloud consoles
- $ Credits (and educational affiliation to get credits)  
- Basic and least-expensive/free-tier/smallest VM configurations
- Compliance to all healthcare related regulations, especially with PHI/PII data

## Oracle Cloud Infrastructure (OCI)

### VM Creation Steps
1. **Compartment**: `briggsp`  
2. **Networking**: VCN with default internet connectivity ?? 
3. **Shape**: `VM.Standard.E2.1.Micro`  ??
4. **Image**: Ubuntu  
5. **Public IP**: Ephemeral  ??
6. **Boot Volume**: Default minimal

**Screenshot**  x collection x
![OCI Create](filename: images/oci-create.png)

---

## Google Cloud Platform (GCP)

### VM Creation Steps
1. Navigate to: **Console → Compute Engine → Create Instance**  
2. **Region/Zone**: `us-east4` (Northern Virginia)  
3. **Machine Type**: `e2-micro` (2 vCPU, 1 core, 1 GB memory)  
4. **Image**: Ubuntu LTS  
5. **Boot Disk**: Default minimal  
6. **Network**: Default VPC with ephemeral public IP  





