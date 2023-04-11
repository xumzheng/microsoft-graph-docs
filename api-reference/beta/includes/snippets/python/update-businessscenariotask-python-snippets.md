---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BusinessScenarioTask()
request_body.@odatatype = '#microsoft.graph.businessScenarioTask'

request_body.title = 'Customer order #12010'

request_body.percentComplete = 20

request_body.priority = 1

businessScenarioProperties = BusinessScenarioProperties()
businessScenarioProperties.externalObjectVersion = '000003'


request_body.businessScenarioProperties = businessScenarioProperties



result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.tasks_by_id('businessScenarioTask-id').patch(request_body = request_body)


```