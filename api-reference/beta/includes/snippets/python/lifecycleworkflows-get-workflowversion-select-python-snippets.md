---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = WorkflowVersionRequestBuilderGetRequestConfiguration();

queryParameters = WorkflowVersionRequestBuilderGetQueryParameters();
queryParameters.select = ["category","displayName","versionNumber","executionConditions"];
queryParameters.expand = ["tasks"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().lifecycleWorkflows().workflowsById('workflow-id').versionsById('workflowVersion-versionNumber').get(requestConfiguration);


```