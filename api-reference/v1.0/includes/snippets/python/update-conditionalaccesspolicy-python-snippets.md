---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConditionalAccessPolicy();
$conditions = new ConditionalAccessConditionSet();
$conditions->setSignInRiskLevels([$conditions->setRiskLevel(new RiskLevel('high'));
$conditions->setRiskLevel(new RiskLevel('medium'));
$conditions->setRiskLevel(new RiskLevel('low'));
]);


$requestBody->setConditions($conditions);


$requestResult = $graphServiceClient->identity()->conditionalAccess()->policiesById('conditionalAccessPolicy-id')->patch($requestBody);


```