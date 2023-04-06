---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = WorkflowsRequestBuilderGetRequestConfiguration(
request_config = WorkflowsRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "category eq 'leaver'"
params['select'] = ["id","category","displayName","isEnabled","isSchedulingEnabled"]
)


result = await client.identityGovernance.lifecycleWorkflows.workflows.get(request_config, headers=request_config)


```