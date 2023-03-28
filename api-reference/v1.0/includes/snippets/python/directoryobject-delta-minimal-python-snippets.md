---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->filter = "isof or isof";
$queryParameters->select = ["microsoft.graph.user/surname","microsoft.graph.group/displayName"];

$headers = [
'Prefer' => 'return=minimal',
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$requestResult = $graphServiceClient->directoryObjects()->delta()->get($requestConfiguration);


```