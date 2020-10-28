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

# Creating support cases 
{: #open-case}

If you experience problems with {{site.data.keyword.Bluemix}}, you can use the [Support Center](https://cloud.ibm.com/unifiedsupport/supportcenter){: external} to create a support case. Users with a Basic, Advanced, or Premium [support plan](/docs/get-support?topic=get-support-support-plans) can create a technical support case by attaching a specific resource or product to the support case to ensure that the case gets to the correct support engineer faster for a more efficient and effective resolution.  
{:shortdesc}

You can also create support cases for issues associated with access (IAM), billing & usage, account, and invoice or sales inquiries. The types of available support depends on the support level of the account. Your support plan also determines the severity level that you can assign to support cases. For more information, see [Case severity and response time](/docs/get-support?topic=get-support-support-case-severity).

Users with a Lite account can also create support cases, but are limited to issues associated with access (IAM), billing & usage, account, and invoice or sales inquiries. Technical support for Lite accounts with free support is provided by the [{{site.data.keyword.Bluemix_notm}} docs](https://cloud.ibm.com/docs){: external} and [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-cloud?tab=Newest){: external}. 

By default, account users don't have access to create, update, search, or view cases. The account owner must provide users access by assigning an Identity and Access Management (IAM) access policy. For more information, see [Assigning user access for working with support cases](/docs/get-support?topic=get-support-access#access).
{:tip}

Complete the following steps to create a support case: 

  1. In the {{site.data.keyword.Bluemix_notm}} console, go to **Support** from the console menu bar.
  1. From the Contact support section, click **Create a case**. 
  1. Select the type of issue that you need help with.
    * To add a resource, select **Your resources**. Select the impacted product, select your resource, and click **Next**.  
    * To add a product, select **All products**. Select the impacted product and clik **Next**. 
    * For all other issues, select the case type, select the problem that's closest to your issue, and click **Next**. 
  1. Complete the required fields.
    * To maintain device security and service security, do not include any device or service credentials within case responses. The response fields are not intended for Personal Information or Sensitive Data. Information entered into these fields is retained to provide the best support experience.
  1. Optional: 
    * Attach files and resources to provide more details about the issue you're experiencing.
    * Add another user to the case if the user is in the account. For more information, see [Adding users to your case management access group](/docs/get-support?topic=get-support-access#add-user-access-group).
    * Select **Email me updates about this case** to receive support case notifications. 
  1. Click **Next**, review your case summary, and click **Submit case**. You will receive email verification for the case. Follow the instructions for further communication on the issue. 

After your support case is created, you can follow its progress on the [Manage cases page](https://{DomainName}/unifiedsupport/cases). 
{: tip}

## Supported file types for cases 
{: #supported-file-types}

When you create a case, you can attach a file. The following file types are supported: 

```
7z, ace, ams, arm, asp, bash, history, bkp, big, bmp, bz2, ca, ca-bundle, ca-crt, cabundle, cap, cer, cert, cfg, cnf, crt, csr, csv, dat, dbs, debug, dib, dmesg, dmp, doc, docx, dotx, dump, email, eml, emz, env, eps, error, evt, evtx, fragment, gif, gz, gz_aa, gz_ab, gz_ac, har, hosts, htaccess, html, iaf, ics, id, img, info, jpb, jpe, jpeg, jpg, key, lic, log, logsm lon02, lst, lzh, mai, md5, mib, mjpg, msg, mso, odp, ods, odt, oft, openssh, out, ovf, ovpn, p7b, p7s, pages, pcap, pcf, pcx, pdb, pem, pfx, pic, pix, png, ppk, ppt, pptx, psd, psp, pspimage, pub_key, rar, raw, rdp, req, rpt, rtf, sjc03-raid-2, sjc03-raid-log-1, snag, sql, ssh, stats, sth, svg, sxc, tar, targz, tbz2, tcpdump, text, tgz, tgz-aa, tgz-ab, tgz-ac, tgz-ad, tgz-ae, tgz-af, tgz-ag, tgz-ah, tgz-ai, tgz-aj, tgz-ak, tgz-ak, tgz-al, tgz-al, tgz-am, tif, tiff, tip, trace, tsv, txt, ufo, vcf, vdx, vsdx, webarchive, wml, wps, wpz, wrf, wri, xcf, xlog, xlr, xls, xis, xism, xisx, xit, xml, xpm, xps, xslic, xz, yaml, zip, zipaa, zipx, zone
```
{: screen}

## Creating a support case by using the API
{: #create-case-api}

You can programmatically open a support case by calling the Case Management API as shown in the following sample request. For detailed information about the API, see [Case Management](https://cloud.ibm.com/apidocs/case-management#casemanagement-createcase){: external}.

```
curl --location --request POST 'support-center.cloud.ibm.com/case-management/v1/cases' --header 'Content-Type: application/json' --header 'Content-Type: text/plain' --data-raw '{ "type": "technical",
  "subject": "Case subject",
  "description": "Case description",
  "severity":4,
   "offering": {
    "name": "Cloud Object Storage",
    "type": {
      "group": "crn_service_name",
      "key": "cloud-object-storage",
      "kind": "service",
      "id": "dff97f5c-bc5e-4455-b470-411c3edbe49c"
    }
  },
  "resources": [
    {
      "crn": "crn:v1:staging:public:cloud-object-storage:global:a/2dded3de4a4d4a098ebd0998be5cc845:723a59c4-9338-43fe-9dc4-e4a87cc78c8e::",
      "note": "Resource note"
    }
  ]
}'
```
{: codeblock}

### Adding a resource to a support case by using the API
{: #add-resource-api}

You can programmatically add a resource to a support case by using the API as shown in the following sample request. For more details, see the [Case Management API reference](https://cloud.ibm.com/apidocs/case-management#casemanagement-createcase){: external}.

```
curl -X PUT '/case-management/v1/cases/{case_number}/resources' -H 'Authorization: TOKEN' -d '{
  "crn": "296878",
  "note": "This resource does not work"
}'
```
{: codeblock}
