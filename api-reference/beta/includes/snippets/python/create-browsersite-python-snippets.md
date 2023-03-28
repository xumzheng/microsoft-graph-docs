---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BrowserSite();
$requestBody->set@odatatype('#microsoft.graph.browserSite');

$requestBody->setWebUrl('www.microsoft.com');

$requestBody->setTargetEnvironment(new BrowserSiteTargetEnvironment('internetexplorer11'));

$requestBody->setComment('A site that opens in InternetExplorer11');

$requestBody->setMergeType(new BrowserSiteMergeType('default'));

$requestBody->setCompatibilityMode(new BrowserSiteCompatibilityMode('default'));

$requestBody->setAllowRedirect(true);



$requestResult = $graphServiceClient->admin()->edge()->internetExplorerMode()->siteListsById('browserSiteList-id')->sites()->post($requestBody);


```