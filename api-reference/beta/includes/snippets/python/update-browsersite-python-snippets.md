---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BrowserSite();
request_body.setWebUrl('www.microsoft.com');

request_body.setTargetEnvironment(BrowserSiteTargetEnvironment('microsoftedge'));

request_body.setMergeType(BrowserSiteMergeType('default'));

request_body.setCompatibilityMode(BrowserSiteCompatibilityMode('default'));

request_body.setAllowRedirect(false);

request_body.setComment('Updating to Edge.');



result = await client.admin.edge.internetExplorerMode.siteListsById('browserSiteList-id').sitesById('browserSite-id').patch(request_body);


```