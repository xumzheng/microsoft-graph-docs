---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BusinessScenarioTask()
request_body.set@odatatype('#microsoft.graph.businessScenarioTask')

request_body.setTitle('Customer order #12010')

request_body.setPercentComplete(20)

request_body.setPriority(1)

businessScenarioProperties = BusinessScenarioProperties()
businessScenarioProperties.setExternalObjectVersion('000003')


request_body.setBusinessScenarioProperties($businessScenarioProperties)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.tasks_by_id('businessScenarioTask-id').patch(request_body, headers=)


```