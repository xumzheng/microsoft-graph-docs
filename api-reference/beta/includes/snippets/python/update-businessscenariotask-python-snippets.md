---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BusinessScenarioTask();
requestBody.set@odatatype('#microsoft.graph.businessScenarioTask');

requestBody.setTitle('Customer order #12010');

requestBody.setPercentComplete(20);

requestBody.setPriority(1);

businessScenarioProperties = BusinessScenarioProperties();
businessScenarioProperties.setExternalObjectVersion('000003');


requestBody.setBusinessScenarioProperties($businessScenarioProperties);


result = awaitclient.solutions().businessScenariosById('businessScenario-id').planner().tasksById('businessScenarioTask-id').patch(requestBody);


```