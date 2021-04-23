---

copyright:

  years: 2020, 2021

lastupdated: "2021-04-22"

keywords: data centers, data center support, datacenter, data center closure

subcollection: get-support

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:external: target="_blank" .external}

# Data center closures in 2021
{: #dc-closure}

As part of the data center modernization strategy for {{site.data.keyword.cloud}}, several data centers and PODs are scheduled to close on 03 September 2021.  
{:shortdesc}

The following data centers and PODs are scheduled to close on 03 September 2021:
* OSL01
* HOU02
* DAL05 – POD2 (other PODs in DAL05 are not impacted)
* WDC01 – POD3 and POD4 (other PODs in WDC01 are not impacted)

To prepare for the data center closures, the following {{site.data.keyword.cloud_notm}} services are ending their service support on the following dates:  

| Service        | Support end date |
|----------------|---------------------------------|
| {{site.data.keyword.cloud_notm}} Databases (ICD) | 01 August 2021 |
| {{site.data.keyword.cos_full_notm}} (COS) | 01 August 2021 |
| {{site.data.keyword.containerlong_notm}} (IKS)  | 30 August 2021 |
| {{site.data.keyword.openshiftlong_notm}} (Managed OpenShift) | 30 August 2021 |
{: caption="Table 1. {{site.data.keyword.cloud_notm}} services that are ending support leading up to data center closure" caption-side="top"}

* The {{site.data.keyword.cloud_notm}} Databases portfolio includes {{site.data.keyword.databases-for-postgresql}}, {{site.data.keyword.databases-for-redis}}, {{site.data.keyword.databases-for-etcd}}, {{site.data.keyword.databases-for-mongodb}}, {{site.data.keyword.databases-for-elasticsearch}}, {{site.data.keyword.databases-for-enterprisedb}}, {{site.data.keyword.databases-for-cassandra}}, and {{site.data.keyword.messages-for-rabbitmq}}. 
* The last date to create new deployments for IKS, COS, and Managed OpenShift services in the OSL01 data center is 01 July 2021.

New products and services can't be provisioned on data centers that are scheduled to be closed. 
{: important}


## Withdrawal of support for some data centers - 2021
{: #withdrawal-support-data-centers-2021}

{{site.data.keyword.cloud_notm}} invests significantly in data center infrastructure. These investments include rolling out 
newer data centers and multizone regions (MZRs) designed to deliver a more resilient architecture with higher levels of 
network throughput and redundancy. For more information, see 
[Locations for resource deployment](/docs/overview?topic=overview-locations).

Part of this modernization strategy is to close older data centers that are unsuitable for upgrading. As this transition 
approaches, help is available to assist you in your migration to modern data centers. For more information, see 
[Migrating resources to a different data center](/docs/account?topic=account-migrate-data-center) or 
[FAQs for migrating resources to a different data center](/docs/account?topic=account-faqs-dc-closure).

The following table shows the locations with the associated data centers and specific PODs that are set to close, and the recommended data centers to which you can migrate.  

| Location      | Data Center to Close |  Migration Options  |
|---------------|----------------------|---------------------|
| Oslo          | OSL01                | FRA02, FRA04, FRA05 | 
| Houston       | HOU02                | DAL10, DAL12, DAL13 | 
| Dallas        | DAL05 – POD2 (other PODs in DAL05 are not impacted)  | DAL10, DAL12, DAL13  | 
| Washington DC | WDC01 – POD3 and POD4 (other PODs in WDC01 are not impacted) | WDC04, WDC06, WDC07 | 
{: caption="Table 2. Data centers that are closing in September 2021" caption-side="top"}

The following table describes important dates that you need to be aware of if you have services that run in the data centers 
that are set to close. You receive notifications if you have services in the data centers that are closing.

| Date           | Data Center Migration Milestone |
|----------------|---------------------------------|
| 03 November 2020 | Official announcement for all impacted clients in the following data centers / PODs: HOU02, DAL05 – POD2, WDC01 – POD3 and POD4. |
| 01 December 2020 | Official announcement for all impacted clients in OSL01 |
| November 2020    | Business Partner available to help clients migrate to a new data center. |
| 01 July 2021     | The last date to create new deployments for IKS, COS, and Managed OpenShift services in OSL01. |
| 01 August 2021   | ICD and COS services end service support. |
| 30 August 2021    | IKS and Managed OpenShift services end service support. |
| 03 September 2021 | OSL01, HOU02, DAL05 - POD2, and WDC01 – POD3 and POD4 data centers are closed; no longer available or supported. Other PODs in DAL05 and WDC01 are not impacted. |
{: caption="Table 3. Timeline for data center migration" caption-side="top"}




