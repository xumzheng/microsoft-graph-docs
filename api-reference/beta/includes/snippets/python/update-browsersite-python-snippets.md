---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BrowserSite();
$requestBody.setWebUrl('www.microsoft.com');

$requestBody.setTargetEnvironment(new BrowserSiteTargetEnvironment('microsoftedge'));

$requestBody.setMergeType(new BrowserSiteMergeType('default'));

$requestBody.setCompatibilityMode(new BrowserSiteCompatibilityMode('default'));

$requestBody.setAllowRedirect(false);

$requestBody.setComment('Updating to Edge.');



$requestResult = $graphServiceClient.admin().edge().internetExplorerMode().siteListsById('browserSiteList-id').sitesById('browserSite-id').patch($requestBody);


```