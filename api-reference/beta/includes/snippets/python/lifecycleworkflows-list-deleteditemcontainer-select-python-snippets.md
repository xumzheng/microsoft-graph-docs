---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = WorkflowsRequestBuilderGetRequestConfiguration()

query_params = WorkflowsRequestBuilderGetQueryParameters()
query_params.select = ["id","category","displayName","description","version"]
query_params.filter = "category eq 'leaver'"

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.deletedItems.workflows.get(request_config)


```