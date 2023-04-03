---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConditionalAccessPolicy();
conditions = ConditionalAccessConditionSet();
conditions.setSignInRiskLevels([conditions.setRiskLevel(RiskLevel('high'));
conditions.setRiskLevel(RiskLevel('medium'));
conditions.setRiskLevel(RiskLevel('low'));
]);


requestBody.setConditions($conditions);


requestResult = graphServiceClient.identity().conditionalAccess().policiesById('conditionalAccessPolicy-id').patch(requestBody);


```