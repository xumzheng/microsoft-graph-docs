---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ListItemRequestBuilderGetRequestConfiguration();

$queryParameters = new ListItemRequestBuilderGetQueryParameters();
$queryParameters.expand = ["fields"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.sitesById('site-id').listsById('list-id').itemsById('listItem-id').get($requestConfiguration);


```