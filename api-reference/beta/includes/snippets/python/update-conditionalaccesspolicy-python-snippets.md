---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
conditions = ConditionalAccessConditionSet()
conditions.SignInRiskLevels([conditions.RiskLevel(RiskLevel('high'))
conditions.RiskLevel(RiskLevel('medium'))
conditions.RiskLevel(RiskLevel('low'))
])


request_body.conditions = conditions



result = await client.identity.conditionalAccess.policies_by_id('conditionalAccessPolicy-id').patch(request_body = request_body)


```