---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = ExecutionScopeRequestBuilder.ExecutionScopeRequestBuilderGetQueryParameters(
				select = ["id"],
)

request_configuration = ExecutionScopeRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').executionScope.get(request_configuration = request_configuration)


```