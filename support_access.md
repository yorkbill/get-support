---

copyright:

  years: 2018,2020

lastupdated: "2020-04-10"

keywords: access to cases, get access for cases, assign cases, watchlist

subcollection: get-support

---


{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:new_window: target="_blank"}

# Assigning user access for working with support cases
{: #access}

By default, users in your account don't have access to create, update, search, or view cases. The account owner must provide users access by assigning an Identity and Access Management (IAM) access policy. Use the Support Center account management service to assign users access to work with support cases. 
{:shortdesc}

When you create a case, you can give other users full access to that case by adding their email on the **Add another person to this case** field. Any added users have access to view, edit, and update only that case in the account. They also receive notifications when the case is updated. 

For classic infrastructure users, the permissions to assign support case access is now available in [migrated classic infrastructure permission access groups](/docs/iam?topic=iam-infrapermission#predefined). The migrated permission access groups do include the IAM policy on the user management service with the viewer role assigned.
{: note}

## Creating an access group for working with cases
{: #creating-access-group}

To streamline the access assignment process, you can take advantage of assigning a policy to users through access groups. Complete the following steps to create an access group with support center service access:

1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Manage** > **Access (IAM)**, select **Access groups**, and click **Create**. 
1. Enter an access group name and description, and click **Create**. 
1. Click **Access policies** > **Assign access**.
1. From the Assign access to account management services section, select **Account management**.
1. Select **Support Center**.
1. Select any combination of roles to assign the wanted access. 
1. Click **Add**, then click **Assign** from the Access summary section.  

| Role          | Action                                                                              | 
|---------------|-------------------------------------------------------------------------------------|
| Viewer        | View and search cases                                                               |
| Editor        | View, search, create, and update cases                                              |
| Administrator | View, search, create, and update cases; manage support center roles for other users |
{: caption="Table 1. Roles and actions for the Support Center service" caption-side="top"}

By default, users with a Support Center service role can access only support cases that they are assigned to unless one of the following conditions is met:

* User list visibility is set to Unrestricted view by the account owner.
* The user is assigned a user management account management service role.

### Assigning access for all support cases in the account
{: #support-view-account}

When you give a user access, they might not have access view all cases in an account. If the account owner sets the user list visibility setting to restricted, users can view only the cases that they create themselves. To ensure that a user can always view or edit all cases in the account, you must assign a second access policy with the viewer role on the User Management service. If you want to ensure that your users can view all support cases in the account, add a policy with the viewer role for the User Management service to your access group:

1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Manage** > **Access (IAM)**, select **Access groups** and select the Group that you want to have access.
1. Click **Access policies** > **Assign access**.
1. Select **Assign access to account management services**.
1. Select **User Management**.
1. Select **Viewer**.
1. Click **Add** and click **Assign** after you review.


## Adding users to your case management access group
{: #add-user-access-group} 

After you create the access group, complete the following steps to add users:

1. From the **Users** tab for your access group, click **Add users**.
1. Select the user that you want to add and click **Add to group**.


## Granting individual users access to cases 
{: #support-user-access}

Using access groups to assign the support center and user management services is the most efficient way for you to assign access, but you can also assign the same permissions to individual users. 

1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Manage** > **Access (IAM)**, and then select **Users**. 
1. Select the user. 
1. Click **Access policies** > **Assign access**.
1. In the Assign user additional access section, select **Account management**.
1. From the What type of access do you want to assign? section, select **Support Center**.
1. Select any combination of roles to assign the wanted access. 
1. Click **Add**, then click **Assign** from the Access summary section.  

