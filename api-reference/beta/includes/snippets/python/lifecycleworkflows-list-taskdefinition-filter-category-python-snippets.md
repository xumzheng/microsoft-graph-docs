---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TaskDefinitionsRequestBuilderGetRequestConfiguration(
query_params = TaskDefinitionsRequestBuilderGetQueryParameters()
query_params.filter = "category has 'joiner'"

)


result = await client.identityGovernance.lifecycleWorkflows.taskDefinitions.get(request_config)


```