---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DevicesRequestBuilderGetRequestConfiguration();

$queryParameters = new DevicesRequestBuilderGetQueryParameters();
$queryParameters->select = ["id","extensionAttributes"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->devices()->get($requestConfiguration);


```