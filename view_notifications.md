---

copyright:

  years: 2019, 2022

lastupdated: "2022-04-01"

keywords: notifications, view notifications, set notifications, iaas notifications, notification icon, header bell, bell icon 

subcollection: get-support

---

{{site.data.keyword.attribute-definition-list}}

# Viewing notifications
{: #viewing-notifications}

The {{site.data.keyword.Bluemix_notm}} [Notifications page](/notifications){: external} is a centralized place to view and control all incidents, maintenance, announcements, and security bulletins. Events that are displayed on the Notifications page are ones that specifically impact users based on the preferences that the account owner or administrator sets.
{: shortdesc}

Pages specific to the {{site.data.keyword.Bluemix_notm}} classic infrastructure are deprecated. The new Notifications page hosts all classic infrastructure notifications. You can view classic infrastructure history for planned and unplanned incidents and announcements on the Notifications page. 
{: note}

To view the page, log in to the {{site.data.keyword.Bluemix_notm}} console, and click the **Notifications** icon ![Notification icon "Notifications"](../icons/Notification.svg) on the menu bar. 

The new notification experience provides enhancements to how users are notified about important changes on the {{site.data.keyword.Bluemix_notm}} platform: 

* The **Notifications** icon ![Notification icon "Notifications"](../icons/Notification.svg) on the {{site.data.keyword.Bluemix_notm}} console shows a red indicator that is only visible when a new notification is available. You can see the details and interact with new and archived notifications.
* The Notifications page is account that is scoped and shows only notifications for the account that is selected on the menu bar. You can switch accounts to view notifications that are affecting a different account. 
* The severity or impact is listed for each notification type. Depending on the notification, you might see severity 1 listed for an unplanned incident notification and high impact that is listed for a planned maintenance notification. 
* You can use the search field to locate a specific notification or filter by a notification type. 
* Navigate to a specific notification by using the unique URL that is associated with each notification. You can save and share the URL with users in the account. 
* You can access the Notifications page with the applied filters to view only applicable notifications. Make sure to save the URL to view the Notifications page with the applied filters. 
* If you want to receive future updates about a specific type of notification, click the **Email** icon next to each notification item in the list. 


## Notification types
{: #notification-types}

The following table describes the different types of notifications that are displayed. 

| Notification Type | Description |
|-------------------|-------------|
| Planned maintenance | Scheduled maintenance that is required to keep the {{site.data.keyword.Bluemix_notm}} platform and infrastructure operating at optimal status. |
| Security bulletins | Announcements about security vulnerabilities and the required actions. |
| Announcements | Updates on new infrastructure features and services in {{site.data.keyword.Bluemix_notm}}. | 
| Incidents | Unexpected impacting events that can cause an outage or restrict functionality. |
| Account | Invitation email, or console notifications for inviting users to the {{site.data.keyword.Bluemix_notm}} platform.  |
{: caption="Table 1. Notification types" caption-side="top"}


## Subscribing to email notifications
{: #subscribe-email-notifications}

You can select whether to receive email notifications about {{site.data.keyword.Bluemix_notm}} platform-related items, such as announcements, billing and usage, additional notification preferences, and ordering. Or, about resource-related items, such as incidents, maintenance, security bulletins and resource activity. Additionally, if you have a Pay-As-You-Go or Subscription account, you can choose whether to receive {{site.data.keyword.Bluemix_notm}} infrastructure service updates about changes, such as OS reloads, assigned IPs, and image and firmware updates. For more information, see [Setting email preferences for notifications](/docs/account?topic=account-email-prefs).

You cannot set email preferences for receiving account type notifications. On the {{site.data.keyword.Bluemix_notm}} [Notifications page](/notifications){: external}, you can use the search field to locate an invitation or filter by the notification type called account. 

Users already present in {{site.data.keyword.Bluemix_notm}} receives an email and a notification with an invitation link. If an email address does not correspond to a known user in {{site.data.keyword.Bluemix_notm}}, an invitation email gets sent to accept, but users can also choose not to accept the invitation. For more information, see [Setting email preferences for notifications](/docs/account?topic=account-email-prefs) and [Inviting users to an account](/docs/account?topic=account-iamuserinv).

The invitations expire after 30 days. New users to {{site.data.keyword.cloud_notm}} can only accept an invitation by using the invitation link that they received through email.
{: note}


## Getting advanced notice for disruptive maintenance
{: #disruptive-maintenance}

{{site.data.keyword.Bluemix_notm}} tries to limit disruptive, required maintenance for Platform as a Service (PaaS) and Infrastructure as a Service (IaaS) offerings. Most maintenance is done in a nondisruptive manner to avoid the impact to your business, but when disruptive maintenance is necessary, we provide as much advanced notice as possible. 

For IaaS offerings, {{site.data.keyword.Bluemix_notm}} provides advanced notice that's dependent on the severity of the impact. The following table defines the types and levels of the possibility of an impact. 

| Possibility of impact | Definition | Advanced Notice Guidelines |
|-----------------------|------------|----------------------------|
| Emergency             | Customer Impacting Event (CIE) | a minimum of 24 hours |
| High                  | Certain, likely, or has the potential to cause an extended or brief service disruption. | a minimum of 30 days |
| Medium                | Low to moderate possibility of a brief disruption. | a minimum of 21 days |
| Low                   | None to negligible chance of a disruption or routine change. No assumed risk or a disruption that is isolated to a single customer. | offering-specific | 
{: caption="Table 2. IaaS offerings impact possibility definitions" caption-side="top"}
