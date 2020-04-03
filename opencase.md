---

copyright:

  years: 2015, 2020

lastupdated: "2020-04-03"

keywords: create case, manage case, open case, start case, ticket

subcollection: get-support

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Working with support cases 
{: #open-case}

If you experience problems with {{site.data.keyword.Bluemix}}, you can use support cases to get help with technical, access (IAM), billing & usage, and invoice or sales inquiry issues. You can create and manage a support case by using the [Support Center](https://cloud.ibm.com/unifiedsupport/supportcenter){: external}. After you submit a support case, the support team investigates the issue based on your type of [support plan](/docs/get-support?topic=get-support-support-plans).
{:shortdesc}

By default, account users don't have access to create, update, search, or view cases. The account owner must provide users access by assigning an Identity and Access Management (IAM) access policy. For more information, see [Assigning user access for working with support cases](/docs/get-support?topic=get-support-access#access).
{:tip}


## Creating support cases
{: #opentechcase}

All users can open a support case, but Lite accounts are unable to open technical support cases. Technical support for Lite accounts with FREE support is provided by the {{site.data.keyword.Bluemix_notm}} docs and [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-cloud?tab=Newest){: external}. 

Complete the following steps to create a support case from the Support Center: 

  1. Click **Support** from the console menu bar.
  1. From the **Contact support** section, click **Create case**. 
  1. Select the type of issue that you need help with. 
  1. Complete the required fields.
  1. Optional: 
    * Attach files that provide more details about the issue you're experiencing.
    * Add another user to the case if the user is in the account. For more information, see [Adding users to your case management access group](/docs/get-support?topic=get-support-access#add-user-access-group).
    * Select **Email me updates about this case** to receive support case notifications. 
  1. Click **Create**. You will receive email verification for the case. Follow the instructions for further communication on the issue. 

You can also create a support case by clicking **View all open cases** from the Recent cases section of the Support page. Then, from the Manage cases page, click **Create new case**. 
{: tip} 

### Supported file types for cases 
{: #supported-file-types}

When you create a case, you can attach a file. The following file types are supported: 

```
7z, ace, ams, arm, asp, bash, history, bkp, big, bmp, bz2, ca, ca-bundle, ca-crt, cabundle, cap, cer, cert, cfg, cnf, crt, csr, csv, dat, dbs, debug, dib, dmesg, dmp, doc, docx, dotx, dump, email, eml, emz, env, eps, error, evt, evtx, fragment, gif, gz, gz_aa, gz_ab, gz_ac, har, hosts, htaccess, html, iaf, ics, id, img, info, jpb, jpe, jpeg, jpg, key, lic, log, logsm lon02, lst, lzh, mai, md5, mib, mjpg, msg, mso, odp, ods, odt, oft, openssh, out, ovf, ovpn, p7b, p7s, pages, pcap, pcf, pcx, pdb, pem, pfx, pic, pix, png, ppk, ppt, pptx, psd, psp, pspimage, pub_key, rar, raw, rdp, req, rpt, rtf, sjc03-raid-2, sjc03-raid-log-1, snag, sql, ssh, stats, sth, svg, sxc, tar, targz, tbz2, tcpdump, text, tgz, tgz-aa, tgz-ab, tgz-ac, tgz-ad, tgz-ae, tgz-af, tgz-ag, tgz-ah, tgz-ai, tgz-aj, tgz-ak, tgz-ak, tgz-al, tgz-al, tgz-am, tif, tiff, tip, trace, tsv, txt, ufo, vcf, vdx, vsdx, webarchive, wml, wps, wpz, wrf, wri, xcf, xlog, xlr, xls, xis, xism, xisx, xit, xml, xpm, xps, xslic, xz, yaml, zip, zipaa, zipx, zone
```
{: screen}


## Managing your support cases 
{: #check-case-status}

All client support issues are documented in support cases. Each support case is assigned a unique case number and a severity level based on the details in the case description. You can use the case number to review your support case progress and update the support case. Updates are recorded in the case notes, which can be found by selecting the specific support case. You can also select a case from the list to add comments and add users from the account to a watchlist so they can receive alerts about a case. 

To view and manage your support cases, use the following steps:

1. Click **Support** from the console.
1. Click **View all open cases**.

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
