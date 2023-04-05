---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BusinessScenarioTask()
request_body.set@odatatype('#microsoft.graph.businessScenarioTask')

request_body.setTitle('Customer order #12010')

request_body.setPercentComplete(0)

request_body.setPriority(5)

target = BusinessScenarioTaskTargetBase()
target.set@odatatype('microsoft.graph.businessScenarioGroupTarget')

target.setTaskTargetKind(PlannerTaskTargetKind('group'))

additionalData = [
'groupId' => '7a339254-4b2b-4410-b295-c890a16776ee', 
];
target.setAdditionalData(additionalData)



request_body.setTarget($target)
businessScenarioProperties = BusinessScenarioProperties()
businessScenarioProperties.setExternalObjectId('Order#12010')

businessScenarioProperties.setExternalContextId('Warehouse-CA-36')

businessScenarioProperties.setExternalObjectVersion('000001')

businessScenarioProperties.setWebUrl('https://ordertracking.contoso.com/view?id=12010')

businessScenarioProperties.setExternalBucketId('deliveryBucket')


request_body.setBusinessScenarioProperties($businessScenarioProperties)


result = await client.solutions_businessScenariosby_id('businessScenario-id')_planner_tasks.post(request_body)


```