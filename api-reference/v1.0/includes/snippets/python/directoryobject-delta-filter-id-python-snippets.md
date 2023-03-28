---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters.filter = "id eq '87d349ed-44d7-43e1-9a83-5f2406dee5bd'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.directoryObjects().delta().get($requestConfiguration);


```