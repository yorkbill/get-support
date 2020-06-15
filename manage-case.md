---

copyright:

  years: 2015, 2020

lastupdated: "2020-06-11"

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
{: #check-case-status}

All client support issues are documented in support cases. Each support case is assigned a unique case number and a severity level based on the details in the case description. You can use the case number to review your support case progress and update the support case. Updates are recorded in the case notes, which can be found by selecting the specific support case. You can also select a case from the list to add comments and add users from the account to a watchlist so they can receive alerts about a case. 


## Viewing support cases
{: #viewing-support-cases}

To view and manage your support cases, use the following steps:

1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Support**.
1. Click **View all** from the Recent support cases widget.

To view closed or resolved cases use the filter option to retrieve cases in any status. If you're a classic infrastructure user, and you don't see a listing of a previous case, go to **View archived cases**. 
{: tip}


## Searching for support cases 
{: #search-options}

From the Manage cases page, you can search for all of your support cases by using query parameters in the search bar. All parameters can be used together and can be entered in any order. 

The following table shows search parameters and their use.
 
| Parameter | Option                                                                           | Rule                                                                         |
|-----------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------|
| number    | target case number                                                               | This parameter can't be used with other parameters. When the `number` parameter is used, all of the other parameters and options ignored. The `number` parameter doesn't autofill the search. You must use the whole case number to execute the search. |
| sort      | number<br>subject<br>severity<br>updatedAt                                       | Only one of the `sort` options can be used at one time. You can use the '~' prefix to reverse the sorting order. |
| status    | new<br>inProgress<br>waitingOnClient<br>resolutionProvided<br>resolved<br>closed | Any number of options can be used. The available options can be entered as `status:new,inProgress` or as `status:new status:inProgress`. |
| page      | target page to view                                                         | If you have several results from your search that spans multiple pages, you can view your results from any result page. For example, to view page 5 out of 10, use `page:5`. |
| pageSize  | 10<br>25<br>50<br>100                                                         | The size of that page to be viewed. The page size refers to the number of results that you want to load. |
{: caption="Table 1. Search query parameters and options" caption-side="top"}

If a term is entered without a parameter, the search results are shown for the support case number and the case subject. 
{: note}

### Query examples
{: #search-query-examples}

You want to search support cases by case number. Enter the following search query:

`number:CS1234567`

You want to search for both new and in progress support cases, limit the results to 25 per page, and displayed by severity. You also know that the case you're looking for isn't going to be within the first couple of pages, so you want to start on page 5. Enter the following search query: 

`status:new,inProgress page:5 pageSize:25 sort:severity`

You want to search for cases by the updated date, but you want to view them from oldest to newest. You also want the status of the support cases to be resolved. 

`sort:~updatedAT status:resolved`
