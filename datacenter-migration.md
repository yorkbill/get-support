---

copyright:

  years: 1994, 2020

lastupdated: "2020-03-03"

keywords: data centers, data center support, Dallas, Seattle, Melbourne, Houston, D2, D6, DAL07, SEA01, H2, MEL01, datacenter

subcollection: get-support

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:external: target="_blank" .external}

# Withdrawal of support for some data centers 
{: #dc-migrate}

<!--Go live for this doc in production is currently March 3, 2020-->
As part of the data center modernization strategy, older data centers in Dallas, Melbourne, and Seattle (DAL07, MEL01, SEA01) are closing on 31 August 2020. In addition, legacy Planet data centers in Dallas and Houston (D2, D6, D7, H2) are also closing on 31 August 2020. You should receive notifications if you have {{site.data.keyword.BluVirtServers_full}} or {{site.data.keyword.baremetal_long}} in the data centers that are closing.
{:shortdesc}

{{site.data.keyword.cloud_notm}} has invested significantly in data center infrastructure in recent years. These investments include rolling out newer data centers and Multizone Regions (MZRs) designed to deliver a more resilient architecture with higher levels of network throughput and redundancy. For more information, see [How do I ensure zero downtime?](/docs/overview?topic=overview-zero-downtime) 

Part of this modernization strategy is to close older data centers that are unsuitable for upgrading. As this transition approaches, help is available to assist you in your migration to modern data centers.


## Help is available
{: #dc-migration-help}

Throughout the data center migration process, help is available from the {{site.data.keyword.IBM_notm}} Client Success team.  

To identify your impacted servers, take advantage of special offers, or learn about recommended configurations, contact the {{site.data.keyword.IBM_notm}} 24x7 Client Success team: 
  * [Live chat](https://www.ibm.com/cloud/data-centers/?focusArea=WCP%20-%20Pooled%20CSM&contactmodule){: external}
  * Phone: (US) 866-597-9687; (EMEA) +31 20 308 0540; (APAC) +65 6622 2231


## Data centers that are closing 31 August 2020
{: #dc-closures-Aug-2020}

The following table shows the locations with the associated data centers that are set to close on 31 August 2020, and the recommended data centers to which you can migrate.  

| Location      | Data centers to be closed                                          |  Recommended data centers |
|---------------|--------------------------------------------------------------------|---------------------------|
| Dallas        | DAL07                                                              | DAL10, DAL12, DAL13       | 
| Melbourne     | MEL01                                                              | SYD01, SYD04, SYD05       |
| Seattle       | SEA01                                                              | DAL10, DAL12, DAL13       |
| Legacy Planet | D2 *(colocation in Dallas)*, D6 and D7 *(Dallas)*, H2 *(Houston)*  | DAL10, DAL12, DAL13       |
{: caption="Table 1. Data centers that are closing on 31 August 2020" caption-side="top"}


## What should I do next?
{: #dc-closure-whats-next}
 
If you have [virtual server instances](/docs/vsi?topic=virtual-servers-getting-started-tutorial), [bare metal servers](/docs/bare-metal?topic=bare-metal-getting-started), or colocation that run on the closing data centers, plan to migrate to a new data center. You must complete the following steps before 31 August 2020. 

1. Identify any virtual server instances or bare metal servers that are currently running on the data centers that are set to close. For more information, see [Help is available](/docs/get-support?topic=get-support-dc-migrate#dc-migration-help) or [How do I determine my current hardware configuration?](/docs/get-support?topic=get-support-dc-migrate#current-hardware) 
2. Order replacement servers in new data centers. For more information, see [Help is available](/docs/get-support?topic=get-support-dc-migrate#dc-migration-help) or [Locations](/docs/get-support?topic=get-support-dc-migrate#mzr-locations) and [Compute configurations](/docs/get-support?topic=get-support-dc-migrate#available-configs). 
3. Migrate your workloads to a new {{site.data.keyword.cloud_notm}} data center before 31 August 2020 to avoid service interruptions. For more information, see [Help is available](/docs/get-support?topic=get-support-dc-migrate#dc-migration-help) or [How do I copy data from my old server to the new one?](/docs/get-support?topic=get-support-dc-migrate#old-server)
4. Cancel your servers after you complete the migration to a new data center. The old servers continue to be invoiced until they're canceled. For more information, see **Cancel** in [Device types and actions](/docs/vsi?topic=virtual-servers-managing-virtual-servers#device-types-and-actions). 

### Timeline for data center migration
{: #dc-timeline}

The following table describes important dates that you need to be aware of if you have servers running in the data centers that are set to close. 

| Date           | Data center migration milestone                                                                                                                                  |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| March 2020     | Data center closure communicated to affected clients by email.                                                                                                   |
| Coming soon!   | Business Partner available to help clients migrate to a new data center.                                                                                         |
| 31 May 2020    | Red Hat Enterprise Linux operating system update infrastructure for patches and OS updates is no longer supported for legacy Planet data centers D2, D6, D7, H2. |
| 31 August 2020 | Data centers closed. DAL07, MEL01, SEA01 are no longer available or supported. Legacy Planet data centers D2, D6, D7, H2 or no longer available or supported.   |
{: caption="Table 2. Timeline for data center migration" caption-side="top"}

### Special offers for migration
{: #dc-timeline}

Transferring data centers can be complex and costly, so the following offers are available:

* Two months free on replacement servers or services in new data centers.  
* The same or a lower price with a same or better configuration.
  * **Bare metal to virtual server**: Migrate to a new {{site.data.keyword.IBM_notm}} virtual server and pay a lower price with the same configuration or next available upgrade. This includes a free architectural consultation with guidance on recommended configurations to help you with the transition and maximize solution performance.
  * **Bare metal to bare metal server**: Migrate to a new bare metal server and pay the same price with the same configuration or next available upgrade.  
  * **Virtual server to virtual server**: For existing virtual servers, pay the same price with the same configuration or next available upgrade.  
<!--* Migration assistance. You can get help to migrate your data to your new server at no cost to you. For more information, see [Help is available](/docs/get-support?topic=get-support-dc-migrate#dc-migration-help). (This bullet point doesn't seem helpful and it also doesn't seem like a special offer.)-->


## Locations available for migration
{: #mzr-locations}

For more information about data centers that are available for you to migrate your current virtual server instances and bare metal servers, see [Locations, regions, and data centers](/docs/overview?topic=overview-locations). The section, [Multizone regions](/docs/overview?topic=overview-locations#mzr-table), provides the current list of multizone regions (MZRs), which feature multiple availability zones for increased fault tolerance. 

For more information about the benefits of MZRs, see [Why Deploy Applications on {{site.data.keyword.cloud_notm}} Availability Zones?](https://www.ibm.com/cloud/blog/why-deploy-applications-on-ibm-cloud-availability-zones){: external}.
{: tip}


## Compute configurations available
{: #available-configs}

You can choose from the following options for deploying virtual server instances and bare metal servers. 

| Compute option                                               | More information                                                                                 |
|--------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| {{site.data.keyword.vsi_is_short}} instances                 | [Planning for VPC instances](/docs/vpc?topic=vpc-vsi_best_practices)                             |
| Classic {{site.data.keyword.virtualmachinesshort}} instances | [Getting started with virtual servers](/docs/vsi?topic=virtual-servers-getting-started-tutorial) |
| Classic {{site.data.keyword.baremetal_short}}                | [Getting started with bare metal servers](/docs/bare-metal?topic=bare-metal-getting-started)     |
{: caption="Table 3. Compute options for migration" caption-side="top"}

For more information about the differences between VPC and Classic infrastructure environments, see [Comparing {{site.data.keyword.cloud_notm}} Classic and VPC infrastructure environments](/docs/overview?topic=overview-compare-infrastructure).
{: tip}


##  FAQs about data center closures and migration
{: #faqs-dc-closure}

###  Why am I required to move to another data center?
{: #required-data}

To continue bringing you the best service, hardware, and connectivity, data centers are continually evaluated to ensure that they meet networking, electrical, and other infrastructure standards. The closing data centers no longer meet the ongoing standards.

### Do I need to be fully migrated by the date listed?
{: #data-list}

Yes. To ensure that you have no interruption in service, we try to allow as much lead time as possible to make the transition easy. 

### Will I need to move to another data center ever again?
{: #move-data}

We constantly evaluate the quality of our sites to bring you the best and most dependable service. It's possible that we might have other moves as we continue to evaluate some of the older sites.

### How do I select which data center to deploy to?
{: #deploy-data}

{{site.data.keyword.IBM_notm}} has more than 60 data centers in locations around the world. View the data center map on our [global data centers page](https://www.ibm.com/cloud/data-centers/){: external} to see the data centers in which you can deploy. 

The following factors might influence which data center you select:
* Proximity to the users of the systems
* Proximity to any other systems that this server needs to communicate with
* Any data policies or regulations that require data to be stored in a specific location

### What sites can I use during the transition period?
{: #transition}

You can use any worldwide {{site.data.keyword.cloud_notm}} site during your transition period, which lasts up to 60 days.

### Are the two free months of transition period resources in addition to my existing server time?
{: #free}

Yes. You can [contact an appropriate support representative](https://www.ibm.com/cloud/data-centers/?focusArea=WCP%20-%20Pooled%20CSM&contactmodule){: external} to help you through the process of acquiring your transition period servers.
<!--Does the customer get two free months of transition period resources? If so we should mention this earlier in the doc, or we could link to where that information can be found-->

### How do I determine my current hardware configuration?
{: #current-hardware}

From your Resource list, you can find system configuration details. Location indicates the data center where the resource is configured. You can view the processor type, for example, Single Intel Xeon E3-1270 (4 Cores, 3.50 GHz). You can also view the amount of memory (RAM), storage, and other data.

To view your current hardware configuration, use the following steps:

1. From the {{site.data.keyword.cloud_notm}} console, click the Menu icon ![Menu icon](../icons/icon_hamburger.svg) > **Resource list** to view your list of resources.
2. Expand **Devices**. 
3. Select the device from the list to see details.  

### How do I determine the utilization of my current hardware?
{: #utilization} 

In general, you need to understand which specific resources within the system are required regarding things like the processor, memory, disk, and network. Having this information can help you better size your new system. For example, a system where memory capacity is frequently overcommitted is likely to benefit from larger memory sizes in the target system that you migrate to.

Most operating systems provide tools that you can use to understand the utilization of your system, for example, vmstat and iostat on Linux or Windows System Performance Monitor. Performance monitoring and tuning is something that you might invest significant time and effort in. 

### How do I compare old and new processors?
{: #old-new}

To compare the specifications of old and new Intel processors, go to [Intel processors product specifications page](https://ark.intel.com/content/www/us/en/ark.html#@Processors){: external}. Newer processors tend to have more processor cores and typically run at slower clock speeds than older variants. 

If you have a workload that is processor-bound, meaning that the performance is limited by the speed of the processor, choose a processor that has fewer cores and a higher clock speed. If you run many workloads that aren't constrained by processor speed, choose a processor with more cores and a similar, or slower, clock speed.

### How do I choose my new operating system?
{: #operating-system}

Compatability and functionality are two of the main influencers when you choose a new operating system. Older versions of operating systems can present challenges with migration. Installation media might not be compatible and the server hardware might not be supported by the older operating system. The best course of action is to compare specs and ensure that the operating system is compatible. Functionality is important because if you have the source code for the application, ensure the necessary development tools and supporting operating system or middleware functions are available on the new platform. In general, Linux type systems are better at supporting older applications on newer versions of the operating system than Windows.
<!--this FAQ doesn't give much information. it should direct the user to do something or link them to a doc that is useful-->

### What bandwidth do I get with my new configuration and is it at the same rate I currently have?
{: #bandwidth}

You receive a current bandwidth package that is most closely related to the package you currently have. The rate for that package is whatever your current rate or package includes.
<!--Is this for virtual server instances and bare metal servers?-->

### How do I copy data from my old server to the new one?
{: #old-server}

You must establish connectivity between the old and new servers and have sufficient storage in the new server. 

* [scp](https://www.ibm.com/support/knowledgecenter/ST5Q4U_1.5.2/com.ibm.storwize.v7000.unified.152.doc/usgr_usng_scp.html){: external} is a good choice to securely copy a file from source to destination. 
* If you need to copy multiple files, [rsync](https://download.samba.org/pub/rsync/rsync.html){: external} over ssh is much faster than scp. rsync also copies directory structures and preserves file permissions. 

Copy only applications and application data between systems. Copying older versions of operating system files to a newer version can cause problems. Shut down databases before you copy them between the systems to ensure that the data is consistent. When migrating database data, ensure that data is migrated in a way that doesn’t limit your options to import it into the new system. Rather than copy database data from system to system, consider exporting it to a format so you can import it to a newer database. Flat text files, CSV files, and other files, provide more options than using proprietary or closed file formats when it comes to moving data between systems. Always test your data migration approaches on a small set of test data before doing the official copying.
<!--FAQs should be quick and link out to more information. This answer wants to provide a lot of detail. If these are important steps, it should be detailed somewhere else.-->

### Do I need to set up my networking again at the new site?
{: #networking}

Most likely, your networking needs to change to work with the new servers and site. If you need help with this process, contact the [{{site.data.keyword.cloud_notm}} support team](/docs/get-support?topic=get-support-dc-migrate#dc-migration-help). For more information about setting up your network, see [Setting up a virtual machine network](/docs/infrastructure/virtualization?topic=Virtualization-setting-up-a-virtual-machine-network).



