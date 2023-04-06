---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.setDisplayName('Policy for risky sign-in block access')

request_body.setState(ConditionalAccessPolicyState('enabled'))

conditions = ConditionalAccessConditionSet()
conditions.setSignInRiskLevels([conditions.setRiskLevel(RiskLevel('high'))
conditions.setRiskLevel(RiskLevel('medium'))
])

conditionsApplications = ConditionalAccessApplications()
conditionsApplications.setIncludeApplications(['All', ])


conditions.setApplications($conditionsApplications)
conditionsUsers = ConditionalAccessUsers()
conditionsUsers.setIncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ])


conditions.setUsers($conditionsUsers)

request_body.setConditions($conditions)
grantControls = ConditionalAccessGrantControls()
grantControls.setOperator('OR')

grantControls.setBuiltInControls([grantControls.setConditionalAccessGrantControl(ConditionalAccessGrantControl('block'))
])


request_body.setGrantControls($grantControls)


result = await client.identity.conditionalAccess.policies.post(request_body, headers=)


```