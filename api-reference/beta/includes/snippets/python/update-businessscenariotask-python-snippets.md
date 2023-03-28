---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new BusinessScenarioTask();
$requestBody.set@odatatype('#microsoft.graph.businessScenarioTask');

$requestBody.setTitle('Customer order #12010');

$requestBody.setPercentComplete(20);

$requestBody.setPriority(1);

$businessScenarioProperties = new BusinessScenarioProperties();
$businessScenarioProperties.setExternalObjectVersion('000003');


$requestBody.setBusinessScenarioProperties($businessScenarioProperties);


$requestResult = $graphServiceClient.solutions().businessScenariosById('businessScenario-id').planner().tasksById('businessScenarioTask-id').patch($requestBody);


```