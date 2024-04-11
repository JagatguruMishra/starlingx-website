---
templateKey: 'software-page'
path: /software
seo:
  title: StarlingX - Open Source Industrial IoT Cloud Platform
  description: StarlingX is an open source project integrating OpenStack, Kubernetes, Ceph, and more to fulfill the requirements of edge computing use cases
  url: https://starlingx.io/software/
  image: /img/android-chrome-192x192.png
  twitterUsername: "@starlingx"
title: Software
subTitle: Development activities in StarlingX
intro:
  video: https://www.youtube.com/embed/72DhrYFIon8
  text: >
    StarlingX is an integration and development project to provide a full software stack suitable 
    to fulfill the strict requirements of edge computing use cases from security to high 
    availability. Beyond integrating well known open source components such as OpenStack modules, 
    Kubernetes, Ceph, OVS-DPDK, and so forth the community is working on new services to fill in 
    the gaps in the open source ecosystem to enhance deployment, maintainability and operation of 
    the software components.
  columns:
    - title: Install the latest image
      link:
        text: mirror.starlingx.cengn.ca
        url: http://mirror.starlingx.cengn.ca/mirror/starlingx/release/
    - title: Get the source code
      link: 
        text: opendev.org/starlingx
        url: https://opendev.org/starlingx
    - title: Install the latest image
      link:
        text: docs.starlingx.io
        url: https://docs.starlingx.io/
---

---

### Configuration Management

In a nutshell you get node configuration and inventory management services with highlight on supporting auto-discovery and configuration of new nodes, which are key when it comes to deploy and manage large number of remote sites some of which might be in areas that are hard to access. This component comes with a Horizon GUI and a CLI to manage the inventory of CPUs, GPUs, memory, huge pages, crypto/compression hardware and so forth.

Check out the code: [opendev.org/starlingx/config/](https://opendev.org/starlingx/config/)

### Fault Management

This framework allows you to set, clear and query custom alarms and logs for significant events for both infrastructure nodes as well as virtual resources such as VMs and networks. You can access the Active Alarm List and Active Alarm Counts Banner on the Horizon GUI.

Check out the code: [opendev.org/starlingx/fault/](https://opendev.org/starlingx/fault/)

### Host Management

The service provides lifecycle management functionality to manage host machines via a REST API interface. This vendor-neutral tool detects host failures and initiates automatic recovery by providing monitoring and alarming for cluster connectivity, critical process failures, resource utilization thresholds and H/W faults. The tool also interfaces with the board management controller (BMC) for out of band reset, power-on/off and H/W sensor monitoring and shares host state with other StarlingX components.

Check out the code: [opendev.org/starlingx/metal/](https://opendev.org/starlingx/metal/)

### Service Management

The Service Manager provides lifecycle management of services by providing high availability (HA) through redundancy models such as N+M or N across multiple nodes. The service supports to use multiple messaging paths to avoid split-brain communication failures as well as active or passive monitoring and to specify the impact of a service failure with a fully data driven architecture.

Check out the code: [opendev.org/starlingx/ha/](https://opendev.org/starlingx/ha/)

### Software Management

This service allows you to deploy software updates for corrective content and also new functionality with a consistent mechanism applicable for all layers of the infrastructure stack – from the kernel all the way up to the OpenStack services. The module can perform rolling upgrades including parallelization and support for host reboot with moving workload off of the node by using live migration. You can access the service in Horizon as well as through a REST API or command line interface.

Check out the code: [opendev.org/starlingx/update/](https://opendev.org/starlingx/update/)
