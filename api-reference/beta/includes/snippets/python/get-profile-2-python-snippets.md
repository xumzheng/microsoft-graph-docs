---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ProfileRequestBuilderGetRequestConfiguration();

$queryParameters = new ProfileRequestBuilderGetQueryParameters();
$queryParameters->expand = ["names($select=first,last)","skills($select=displayName)"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->profile()->get($requestConfiguration);


```