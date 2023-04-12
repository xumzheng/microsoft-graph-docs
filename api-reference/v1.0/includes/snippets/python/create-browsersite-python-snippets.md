---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSite()
request_body.@odatatype = '#microsoft.graph.browserSite'

request_body.webUrl = 'www.microsoft.com'

request_body.TargetEnvironment(BrowserSiteTargetEnvironment('internetexplorer11'))

request_body.comment = 'A site that opens in InternetExplorer11'

request_body.MergeType(BrowserSiteMergeType('default'))

request_body.CompatibilityMode(BrowserSiteCompatibilityMode('default'))

request_body.allowRedirect = true




result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sites.post(request_body = request_body)


```