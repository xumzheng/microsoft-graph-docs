---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = WorkflowRequestBuilder.WorkflowRequestBuilderGetQueryParameters(
		select = ["id","category","displayName","description","version","executionConditions"],
)

request_configuration = WorkflowRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.lifecycleWorkflows.deletedItems.workflows_by_id('workflow-id').get(request_configuration = request_configuration)


```