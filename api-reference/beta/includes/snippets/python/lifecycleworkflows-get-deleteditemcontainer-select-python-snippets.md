---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = WorkflowRequestBuilderGetRequestConfiguration()

query_params = WorkflowRequestBuilderGetQueryParameters()
query_params.select = ["id","category","displayName","description","version","executionConditions"]

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.deletedItems.workflowsById('workflow-id').get(request_config)


```