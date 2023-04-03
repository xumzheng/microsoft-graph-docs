---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = WorkflowsRequestBuilderGetRequestConfiguration();

queryParameters = WorkflowsRequestBuilderGetQueryParameters();
queryParameters.filter = "category eq 'leaver'";
queryParameters.select = ["id","category","displayName","isEnabled","isSchedulingEnabled"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().lifecycleWorkflows().workflows().get(requestConfiguration);


```