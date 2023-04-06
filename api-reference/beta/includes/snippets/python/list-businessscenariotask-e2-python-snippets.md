---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TasksRequestBuilderGetRequestConfiguration(
request_config = TasksRequestBuilderGetRequestConfiguration(query_params=query_params = TasksRequestBuilderGetQueryParameters()
query_params.filter = "businessScenarioProperties/externalContextId eq 'Warehouse-CA-36'"

)
query_params = TasksRequestBuilderGetQueryParameters()
query_params.filter = "businessScenarioProperties/externalContextId eq 'Warehouse-CA-36'"

)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.tasks.get(request_config, headers=request_config)


```