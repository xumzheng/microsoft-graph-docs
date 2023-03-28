---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new GroupRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupRequestBuilderGetQueryParameters();
$queryParameters.select = ["*","parentSiteId"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.sitesById('site-id').termStore().groupsById('group-id').get($requestConfiguration);


```