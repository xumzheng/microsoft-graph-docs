---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSite()
request_body.webUrl = 'www.microsoft.com'

request_body.TargetEnvironment(BrowserSiteTargetEnvironment('microsoftedge'))

request_body.MergeType(BrowserSiteMergeType('default'))

request_body.CompatibilityMode(BrowserSiteCompatibilityMode('default'))

request_body.allowRedirect = false

request_body.comment = 'Updating to Edge.'




result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sites_by_id('browserSite-id').patch(request_body = request_body)


```