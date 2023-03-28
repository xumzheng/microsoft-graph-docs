---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new WorkflowsRequestBuilderGetRequestConfiguration();

$queryParameters = new WorkflowsRequestBuilderGetQueryParameters();
$queryParameters.select = ["id","category","displayName","description","version"];
$queryParameters.filter = "category eq 'leaver'";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.identityGovernance().lifecycleWorkflows().deletedItems().workflows().get($requestConfiguration);


```