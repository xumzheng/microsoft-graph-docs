---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new SessionsRequestBuilderGetRequestConfiguration();

$queryParameters = new SessionsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["segments"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->communications()->callRecordsById('callRecord-id')->sessions()->get($requestConfiguration);


```