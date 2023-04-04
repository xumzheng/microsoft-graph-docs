---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BrowserSite();
request_body.set@odatatype('#microsoft.graph.browserSite');

request_body.setWebUrl('www.microsoft.com');

request_body.setTargetEnvironment(BrowserSiteTargetEnvironment('internetexplorer11'));

request_body.setComment('A site that opens in InternetExplorer11');

request_body.setMergeType(BrowserSiteMergeType('default'));

request_body.setCompatibilityMode(BrowserSiteCompatibilityMode('default'));

request_body.setAllowRedirect(true);



result = await client.admin.edge.internetExplorerMode.siteListsById('browserSiteList-id').sites.post(request_body);


```