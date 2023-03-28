---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CallRecordRequestBuilderGetRequestConfiguration();

$queryParameters = new CallRecordRequestBuilderGetQueryParameters();
$queryParameters.expand = ["sessions($expand=segments)"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.communications().callRecordsById('callRecord-id').get($requestConfiguration);


```