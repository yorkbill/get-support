---

copyright:

  years: 2019, 2020

lastupdated: "2020-03-09"

keywords: cir, impacting event, services, advanced customer support, 

---


{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:new_window: target="_blank"}

# Customer Incident Report (edited)
{: #customer-incident-report}

{{site.data.keyword.Bluemix}} works hard to maintain high availability of infrastructure and cloud services. If you're impacted by any event that disrupts your service delivery, a Customer Incident Report (CIR) can be provided to let you know how services were impacted and how the issue is being resolved. 
{:shortdesc}

After you create a support case, you can view updates about your impacting event from the Manage cases page. For more information, see [Managing your support cases](/docs/get-support?topic=get-support-open-case#check-case-status). If the scope of an impacting event is of a larger enterprise-wide scope, a CIR is provided upon request. 
{: note}


## Details about the Customer Incident Report (CIR)
{: #details-customer-incident-report}

CIR's are provided for larger, enterprise-level issues. They are updates that provide a Root Cause Analysis (RCA) which is the process for determining the underlying cause of a Customer Impacting Event (CIE). Smaller issues that don't affect {{site.data.keyword.Bluemix_notm}} at an enterprise level don't provide an RCA or CIR. The Advanced Customer Support (ACS) team that mitigates the issue still provides updates, but they're not a formal RCA. 

Larger enterprise-wide issues are events that typically impact multiple user environments or regions. Due to the scope and impact of enterprise issues, {{site.data.keyword.Bluemix_notm}} requires a thorough RCA and the CIR is a summary report for the findings of the investigation. 

RCA investigations are complex and involve program review, feedback from product specialists, multiple inter-related cloud services, and vendor discussions. If the CIR can't be delivered within the Service Level Objective (SLO), an interim CIR is provided within the five business day SLO. For more information about SLO, see [Case severity and initial response times](/docs/get-support?topic=get-support-support-case-severity#support-case-severity). 

The interim CIR document provides the current findings of the ongoing RCA, the next investigative steps, and a timeline for the next expected update. Depending on the complexity of the issue, more than one interim CIR might be required before the final version is available. The Service team (SRE) determines when the CIR is available.  

The following image shows the process for receiving a CIR. 

![Flowchart for receiving customer incident report updates.](images/CIRimage.png "Customer incident report flowchart"){: caption="Figure 1. Workflow for getting customer incident report updates." caption-side="bottom"}


## Requesting a Customer Incident Report (CIR)
{: #requesting-customer-incident-report}

A CIR must be requested by using one of the following methods: 

* Create a case requesting a CIR
* Request a CIR within the case description
* Update your case with a request for a CIR

To create a case, go to [Create a case](https://{DomainName}/unifiedsupport/cases/add), or to update your case, go to [Manage cases](https://{DomainName}/unifiedsupport/cases).

After the ACS team receives your request for a CIR, they will initiate the CIR process if the issue was caused by a CIE. When it's available, your CIR is provided with a PDF copy that is attached to your support case.


