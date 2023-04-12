---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetPlanPostRequestBody()
target = BusinessScenarioTaskTargetBase()
target.@odatatype = 'microsoft.graph.businessScenarioGroupTarget'

target.TaskTargetKind(PlannerTaskTargetKind('group'))

additionalData = [
'groupId' => '7a339254-4b2b-4410-b295-c890a16776ee', 
];
target.additionaldata(additionalData)



request_body.target = target



result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.getPlan.post(request_body = request_body)


```