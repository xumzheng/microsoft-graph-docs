---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ItemsRequestBuilderGetRequestConfiguration();

$queryParameters = new ItemsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["fields(select=Name,Color,Quantity)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.sitesById('site-id').listsById('list-id').items().get($requestConfiguration);


```