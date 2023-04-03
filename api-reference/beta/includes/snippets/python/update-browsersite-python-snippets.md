---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BrowserSite();
requestBody.setWebUrl('www.microsoft.com');

requestBody.setTargetEnvironment(BrowserSiteTargetEnvironment('microsoftedge'));

requestBody.setMergeType(BrowserSiteMergeType('default'));

requestBody.setCompatibilityMode(BrowserSiteCompatibilityMode('default'));

requestBody.setAllowRedirect(false);

requestBody.setComment('Updating to Edge.');



requestResult = graphServiceClient.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').sitesById('browserSite-id').patch(requestBody);


```