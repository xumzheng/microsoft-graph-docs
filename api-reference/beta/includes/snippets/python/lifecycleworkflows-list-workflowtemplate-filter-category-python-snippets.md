---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = WorkflowTemplatesRequestBuilder.WorkflowTemplatesRequestBuilderGetQueryParameters(
		filter = "category eq 'leaver'",
)

request_configuration = WorkflowTemplatesRequestBuilder.WorkflowTemplatesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.lifecycleWorkflows.workflowTemplates.get(request_configuration = request_configuration)


```