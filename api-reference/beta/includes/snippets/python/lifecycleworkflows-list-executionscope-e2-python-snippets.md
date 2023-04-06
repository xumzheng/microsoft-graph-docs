---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ExecutionScopeRequestBuilderGetRequestConfiguration(
request_config = ExecutionScopeRequestBuilderGetRequestConfiguration(query_params=params['select'] = ["id"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').executionScope.get(request_config, headers=request_config)


```