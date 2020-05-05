---

copyright:

  years: 2015, 2020

lastupdated: "2020-05-05"

keywords: help managing cases, resolve issues managing cases, trouble working with cases, support center, help support center, resolve issues support center, help getting support, help support 

subcollection: get-support

---


{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}


# Troubleshooting for getting support
{: #Supportcases}

You might encounter problems creating and managing {{site.data.keyword.Bluemix}} support cases, or general problems as you use the support center. In many cases, you can recover from these problems by following a few easy steps.
{:shortdesc}

## Why can't I create or edit support cases? 
{: #ts_service_broker}

You can't create or edit an {{site.data.keyword.Bluemix_notm}} support case, and you receive an error message that you don't have the appropriate access. 
{:shortdesc}

When you try to create a case the following error message is displayed:   
{: tsSymptoms}

`Looks like you don't have access to create cases for this account.`

General problems with accessing and managing support cases might be caused by 
not having the Identity and Access Management (IAM) access policy for the Support Center account management service. You must be assigned the editor or administrator role on the support center account management service to create cases. 
{: tsCauses}

The account owner, an administrator on the support center service, or the administrator on all account management services can assign an IAM policy on support center to manage cases. 
{: tsResolve}

If you're the account owner or an administrator of the Support Center, complete the following steps to create an access policy for working with support cases:

1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Manage** > **Access (IAM)** and select **Users**.
1. Select a username, and click **Access policies**. 
1. Click **Assign Access**. 
1. From the Assign users additional access section, select **Account management**.
1. For the type of access that you want to assign, select **Support Center**. 
1. Select a role to define the level of access for the user. The user needs the Editor or Administrator role to view, search, create, and update support cases. 


## Why can't I view all cases in the account?
{: #ts_viewcasedetails}

You can't view all of the cases in the account because you don't have access to view all users in the account. 
{:shortdesc}

When you try to view the support cases that are associated with the account, you can't see all open cases. You can view users that you invited to the account, users with which you share a Cloud Foundry org membership, and users who are in your classic infrastructure user hierarchy.  
{: tsSymptoms}

The account owner set the [user list visibility setting](/docs/iam?topic=iam-userlistview#userlistview) to restricted, and you don't have the required access to view all cases in the account. 

You must be assigned an IAM policy with at least the Viewer role on the User management account management service in addition to your Support Center account management service access policy. To view your current access, in the {{site.data.keyword.Bluemix_notm}} console, go to **Manage** > **Access (IAM)**, and select your name from the **Users** page. Click the **Access policies** tab. 
{: tsCauses}

To resolve the issue, contact the account owner to request the appropriate access. 
{: tsResolve}


## Why can't I find a case that I previously created? 
{: #ts_viewarchivedcase}

You can't find your cases that you created before the migration from SoftLayer to the enhanced {{site.data.keyword.Bluemix_notm}} experience. 
{:shortdesc}

You can't find any cases that you created before 2018 December 2 on the Manage cases page. 
{: tsSymptoms}

Cases that were opened before 2018 December 2 are visible only as archived cases.
{: tsCauses}

To view your cases, in the {{site.data.keyword.Bluemix_notm}} console, go to **Support** and click **View all** from the Recent support cases widget.
{: tsResolve} 


## Why can't I create a technical support case? 
{: #ts_tech-support-case}

You can't create a technical support case.
{:shortdesc}

You can create cases that are related to access management, accounts, and billing and usage only. 
{: tsSymptoms}

Technical cases can be created only by accounts with advanced and premium support. If you have a Lite account, you must upgrade your account to create a technical support case. 
{: tsCauses}

To update your support plan, go to [{{site.data.keyword.Bluemix_notm}} support](https://www.ibm.com/cloud/support){: external}, and click **Contact us**. From there, you can communicate with an expert through chat, phone, or email.
{: tsResolve}


## Why can't I find help information in the Support Center for my services? 
{: #supportcenter-service}

You can't find any help information that's tailored to the services that are in your account. 
{:shortdesc}

The Support Center doesn't include My products topics, common tasks, or FAQs that are specific to the services that you're working with. 
{: tsSymptoms}

Not all services provide personalized help information in the Support Center. 
{: tsCauses}

The Support Center is updated as help information for more services becomes available. In the meantime, you can explore the [{{site.data.keyword.Bluemix}} FAQ library](https://cloud.ibm.com/docs/faqs) to view FAQs for your services that aren't highlighted in the Support Center.
{: tsResolve}
