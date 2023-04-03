---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConditionalAccessPolicy();
conditions = ConditionalAccessConditionSet();
conditions.setSignInRiskLevels([conditions.setRiskLevel(RiskLevel('high'));
conditions.setRiskLevel(RiskLevel('medium'));
conditions.setRiskLevel(RiskLevel('low'));
]);


requestBody.setConditions($conditions);


result = await client.identity().conditionalAccess().policiesById('conditionalAccessPolicy-id').patch(requestBody);


```