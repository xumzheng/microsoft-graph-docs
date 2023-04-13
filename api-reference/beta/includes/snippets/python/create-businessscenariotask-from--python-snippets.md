---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BusinessScenarioTask()
request_body.@odatatype = '#microsoft.graph.businessScenarioTask'

request_body.title = 'Customer order #12010'

request_body.percent_complete = 0

request_body.priority = 5

target = BusinessScenarioTaskTargetBase()
target.@odatatype = 'microsoft.graph.businessScenarioGroupTarget'

target.TaskTargetKind(PlannerTaskTargetKind('group'))

additionalData = [
'groupId' => '7a339254-4b2b-4410-b295-c890a16776ee', 
];
target.additionaldata(additionalData)



request_body.target = target
business_scenario_properties = BusinessScenarioProperties()
businessScenarioProperties.externalObjectId = 'Order#12010'

businessScenarioProperties.externalContextId = 'Warehouse-CA-36'

businessScenarioProperties.externalObjectVersion = '000001'

businessScenarioProperties.webUrl = 'https://ordertracking.contoso.com/view?id=12010'

businessScenarioProperties.externalBucketId = 'deliveryBucket'


request_body.business_scenario_properties = businessScenarioProperties



result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.tasks.post(request_body = request_body)


```