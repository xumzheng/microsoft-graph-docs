---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = WorkflowTemplatesRequestBuilderGetRequestConfiguration(
request_configuration = WorkflowTemplatesRequestBuilderGetRequestConfiguration(query_params=query_params = WorkflowTemplatesRequestBuilderGetQueryParameters()
query_params['filter'] = "category eq 'leaver'"

)
query_params = WorkflowTemplatesRequestBuilderGetQueryParameters()
query_params['filter'] = "category eq 'leaver'"

)


result = await client.identityGovernance.lifecycleWorkflows.workflowTemplates.get(request_configuration)


```