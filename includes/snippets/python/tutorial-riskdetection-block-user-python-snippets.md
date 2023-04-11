---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.displayName = 'Policy for risky sign-in block access'

request_body.State(ConditionalAccessPolicyState('enabled'))

conditions = ConditionalAccessConditionSet()
conditions.SignInRiskLevels([conditions.RiskLevel(RiskLevel('high'))
conditions.RiskLevel(RiskLevel('medium'))
])

conditionsApplications = ConditionalAccessApplications()
conditionsApplications.IncludeApplications(['All', ])


conditions.applications = conditionsApplications
conditionsUsers = ConditionalAccessUsers()
conditionsUsers.IncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ])


conditions.users = conditionsUsers

request_body.conditions = conditions
grantControls = ConditionalAccessGrantControls()
grantControls.operator = 'OR'

grantControls.BuiltInControls([grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('block'))
])


request_body.grantControls = grantControls


request_configuration = PoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identity.conditionalAccess.policies.post(request_body = request_body)


```