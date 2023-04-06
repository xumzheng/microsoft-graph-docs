---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TasksRequestBuilderGetRequestConfiguration(
request_config = TasksRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "location/microsoft.graph.businessScenarioGroupTarget/groupId eq '7a339254-4b2b-4410-b295-c890a16776ee'"
)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.tasks.get(request_config, headers=request_config)


```