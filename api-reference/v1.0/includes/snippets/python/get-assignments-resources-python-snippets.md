---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AssignmentsRequestBuilderGetQueryParameters();
$queryParameters->expand = ["resources"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->education()->classesById('educationClass-id')->assignments()->get($requestConfiguration);


```