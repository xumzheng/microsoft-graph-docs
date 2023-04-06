---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetPlanPostRequestBody()
target = BusinessScenarioTaskTargetBase()
target.set@odatatype('microsoft.graph.businessScenarioGroupTarget')

target.setTaskTargetKind(PlannerTaskTargetKind('group'))

additionalData = [
'groupId' => '7a339254-4b2b-4410-b295-c890a16776ee', 
];
target.setAdditionalData(additionalData)



request_body.setTarget($target)

request_config = GetPlanRequestBuilderPostRequestConfiguration(
request_config = GetPlanRequestBuilderPostRequestConfiguration(query_params=)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.getPlan.post(request_body, headers=)


```