---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = WorkflowTemplatesRequestBuilderGetRequestConfiguration()

query_params = WorkflowTemplatesRequestBuilderGetQueryParameters()
query_params.filter = "category eq 'leaver'"

request_config.queryParameters = query_params


result = await client.identityGovernance.lifecycleWorkflows.workflowTemplates.get(request_config)


```