---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.displayName = 'Require MFA to EXO from non-compliant devices.'

request_body.State(ConditionalAccessPolicyState('enabled'))

conditions = ConditionalAccessConditionSet()
conditionsApplications = ConditionalAccessApplications()
conditionsApplications.IncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ])


conditions.applications = conditionsApplications
conditionsUsers = ConditionalAccessUsers()
conditionsUsers.IncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ])


conditions.users = conditionsUsers

request_body.conditions = conditions
grantControls = ConditionalAccessGrantControls()
grantControls.operator = 'OR'

grantControls.BuiltInControls([grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'))
])


request_body.grantControls = grantControls


request_configuration = PoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identity.conditionalAccess.policies.post(request_body = request_body)


```