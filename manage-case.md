---

copyright:

  years: 2015, 2020

lastupdated: "2020-10-28"

keywords: create case, manage case, open case, start case, ticket

subcollection: get-support

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Managing your support cases
{: #managing-support-cases}

Each support case is assigned a unique number and severity level based on the details in the case description. You can use the case number to track the progress of your reported issue, leave feedback, or update the support case. Updates and feedback are recorded in the case notes, which you can find by selecting the specific support case. You can also add users in your account to a watchlist so they can receive alerts about a case. 
{: shortdesc}

To view and manage your support cases, go to the [Manage cases page](https://{DomainName}/unifiedsupport/cases). 

If you're a classic infrastructure user, and you don't see a listing of a previous case, click **View classic infrastructure cases**. 
{: tip}


## Searching for support cases 
{: #search-options}

From the Manage cases page, you can search for all of your support cases by using query parameters in the search bar. You can use all parameters together and enter them in any order.

See the following table for details about the search parameters: 
 
| Parameter | Option                                                                           | Rule                                                                         |
|-----------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| `number`    | target case number                                                               | This parameter can't be used with other parameters. When the `number` parameter is used, all of the other parameters and options ignored. The `number` parameter doesn't autofill the search. You must use the whole case number to execute the search. |
| `sort`      | number<br>subject<br>severity<br>updatedAt                                       | Only one of the `sort` options can be used at one time. You can use the `~` prefix to reverse the sorting order. |
| `status`    | new<br>inProgress<br>waitingOnClient<br>resolutionProvided<br>resolved<br>closed | Any number of options can be used. The available options can be entered as `status:new,inProgress` or as `status:new status:inProgress`. |
| `page`      | target page to view                                                         | If you have several results from your search that spans multiple pages, you can view your results from any result page. For example, to view page 5 out of 10, use `page:5`. |
| `pageSize`  | 10<br>25<br>50<br>100                                                         | The size of that page to be viewed. The page size refers to the number of results that you want to load. |
{: caption="Table 1. Search query parameters and options" caption-side="top"}

If you enter a term without a parameter, the search results are shown for the support case number and the case subject. 
{: note}

### Query examples
{: #search-query-examples}

Enter the following query to search support cases by case number:

`number:CS1234567`

You might want to search for both new and in progress support cases, limit the results to 25 per page, and displayed by severity. You also know that the case you're looking for isn't going to be within the first couple of pages, so you want to start on page 5. Enter the following search query: 

`status:new,inProgress page:5 pageSize:25 sort:severity`

Enter the following query to view all resolved cases based on when they were last updated: 

`sort:~updatedAT status:resolved`

### Support case status types
{: #search-case-status}

When your response to an update in your support case is needed, the status is displayed as `Waiting on client`. If you don't provide a response within 7 days, the status is updated to `Resolved`. The case is then closed if there is still no response after 7 more days. For a description of each status type, see the following table:

| Status                | Description |
|-----------------------|------------|
| New                 | A created case that hasn't yet been viewed by a support engineer. |
| In progress         | A case that is under review. |
| Waiting on client   | The support engineer has left an inquiry on the case that needs the user's response. |
| Resolution provided | The support engineer provided a resolution that the user needs to perform. |
| Resolved            | The support case is considered finished and ready to be closed. |
| Closed              | Case is closed by a support engineer and can't be reopened. | 
{: caption="Table 2. Support case status types" caption-side="top"}


## Viewing support cases by using the API
{: #viewing-case-api}

You can programmatically view a support case by using the API as shown in the following sample request. For more details, see the [Case Management API](https://cloud.ibm.com/apidocs/case-management#casemanagement-createcase){: external}.

To view by the content of the IAM token, see the following sample:

```
curl -X GET 'https://support-center.cloud.ibm.com/case-management/v1/cases?offset=0&limit=10&status=new,in_progress,waiting_on_client,resolution_provided' -H 'Authorization: TOKEN' \
```
{: codeblock}

To view a case specified by the case number, see the following sample:

```
curl -X GET '/case-management/v1/cases/{case_number}?fields=number,updated_at,resources' -H 'Authorization: TOKEN' 
```
{: codeblock}


## Updating support cases by using the API
{: #updating-case-api}

The following sample request shows how to programmatically update a support case. For more details, see the [Case Management API](https://cloud.ibm.com/apidocs/case-management#casemanagement-createcase){: external}.

```
curl -X PUT '/case-management/v1/cases/{case_number}/status' -H 'Authorization: TOKEN' -d '{
  "action": "resolve",
  "comment": "The issue is resolved. Thank you!",
  "resolution_code": 1
}'
```
{: codeblock}

## Adding comments to support cases by using the API
{: #comment-case-api}

The following sample request shows how to programmatically add a comment to a support case. For more details, see the [Case Management API](https://cloud.ibm.com/apidocs/case-management#casemanagement-createcase){: external}.

```
curl -X PUT '/case-management/v1/cases/{case_number}/comments' -H 'Authorization: TOKEN' -d '{
  "comment": "Test comment api"
}'
```
{: codeblock}
