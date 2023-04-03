---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BrowserSite();
requestBody.set@odatatype('#microsoft.graph.browserSite');

requestBody.setWebUrl('www.microsoft.com');

requestBody.setTargetEnvironment(BrowserSiteTargetEnvironment('internetexplorer11'));

requestBody.setComment('A site that opens in InternetExplorer11');

requestBody.setMergeType(BrowserSiteMergeType('default'));

requestBody.setCompatibilityMode(BrowserSiteCompatibilityMode('default'));

requestBody.setAllowRedirect(true);



result = await client.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').sites().post(requestBody);


```