---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = BusinessScenarioTask();
requestBody.set@odatatype('#microsoft.graph.businessScenarioTask');

requestBody.setTitle('Customer order #12010');

requestBody.setPercentComplete(0);

requestBody.setPriority(5);

target = BusinessScenarioTaskTargetBase();
target.set@odatatype('microsoft.graph.businessScenarioGroupTarget');

target.setTaskTargetKind(PlannerTaskTargetKind('group'));

additionalData = [
'groupId' => '7a339254-4b2b-4410-b295-c890a16776ee', 
];
target.setAdditionalData(additionalData);



requestBody.setTarget($target);
businessScenarioProperties = BusinessScenarioProperties();
businessScenarioProperties.setExternalObjectId('Order#12010');

businessScenarioProperties.setExternalContextId('Warehouse-CA-36');

businessScenarioProperties.setExternalObjectVersion('000001');

businessScenarioProperties.setWebUrl('https://ordertracking.contoso.com/view?id=12010');

businessScenarioProperties.setExternalBucketId('deliveryBucket');


requestBody.setBusinessScenarioProperties($businessScenarioProperties);


requestResult = graphServiceClient.solutions().businessScenariosById('businessScenario-id').planner().tasks().post(requestBody);


```