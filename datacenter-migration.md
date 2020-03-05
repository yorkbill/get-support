---

copyright:

  years: 1994, 2020

lastupdated: "2020-03-05"

keywords: data centers, data center support, Dallas, Seattle, Melbourne, Houston, D2, D6, DAL07, SEA01, H2, MEL01, datacenter

subcollection: get-support

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Withdrawal of support for some data centers 
{: #dc-migrate}

As part of the data center modernization strategy, older data centers in Dallas, Melbourne, and Seattle (DAL07, MEL01, SEA01) are closing on 31 August 2020. In addition, legacy Planet data centers in Dallas and Houston (D2, D6, D7, H2) are also closing on 31 August 2020. 
{:shortdesc}

{{site.data.keyword.cloud_notm}} invests significantly in data center infrastructure. These investments include rolling out newer data centers and Multizone Regions (MZRs) designed to deliver a more resilient architecture with higher levels of network throughput and redundancy. For more information, see [How do I ensure zero downtime?](/docs/overview?topic=overview-zero-downtime)

Part of this modernization strategy is to close older data centers that are unsuitable for upgrading. As this transition approaches, help is available to assist you in your migration to modern data centers. For information about migrating your data center, see [Migrating resources to a different data center](/docs/resources?topic=resources-migrate-data-center) or [FAQs for data center closures and migration](/docs/resources?topic=resources-faqs-dc-closure).
{: note}


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

The following table describes important dates that you need to be aware of if you have services that run in the data centers that are set to close. You should receive notifications if you have services in the data centers that are closing.

| Date           | Data center migration milestone                                                                                                                                  |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| March 2020     | Data center closure communicated to affected clients by email.                                                                                                   |
| Coming soon!   | Business Partner available to help clients migrate to a new data center.                                                                                         |
| 31 May 2020    | Red Hat Enterprise Linux operating system update infrastructure for patches and OS updates is no longer supported for legacy Planet data centers D2, D6, D7, H2. |
| 31 August 2020 | Data centers closed. DAL07, MEL01, SEA01 are no longer available or supported. Legacy Planet data centers D2, D6, D7, H2 are no longer available or supported.   |
{: caption="Table 2. Timeline for data center migration" caption-side="top"}





