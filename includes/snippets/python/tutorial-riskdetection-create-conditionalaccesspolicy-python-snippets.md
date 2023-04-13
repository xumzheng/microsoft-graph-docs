---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.displayName = 'Policy for risky sign-in'

request_body.State(ConditionalAccessPolicyState('enabled'))

conditions = ConditionalAccessConditionSet()
conditions.SignInRiskLevels([conditions.RiskLevel(RiskLevel('high'))
conditions.RiskLevel(RiskLevel('medium'))
])

conditions_applications = ConditionalAccessApplications()
conditionsApplications.IncludeApplications(['All', ])


conditions.applications = conditionsApplications
conditions_users = ConditionalAccessUsers()
conditionsUsers.IncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ])


conditions.users = conditionsUsers

request_body.conditions = conditions
grant_controls = ConditionalAccessGrantControls()
grantControls.operator = 'OR'

grantControls.BuiltInControls([grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'))
])


request_body.grant_controls = grantControls



result = await client.identity.conditionalAccess.policies.post(request_body = request_body)


```