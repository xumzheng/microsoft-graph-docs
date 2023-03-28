---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedOperationEventsRequestBuilderGetQueryParameters();
$queryParameters.filter = "requestType eq 'Activate'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.privilegedOperationEvents().get($requestConfiguration);


```