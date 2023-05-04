---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Conditional_access_policy()
request_body.display_name = 'Policy for risky sign-in'

request_body.state(ConditionalAccessPolicyState.Enabled('conditionalaccesspolicystate.enabled'))

conditions = Conditional_access_condition_set()
conditions.SignInRiskLevels([conditions.risklevel(RiskLevel.High('risklevel.high'))
conditions.risklevel(RiskLevel.Medium('risklevel.medium'))
])

conditionsapplications = Conditional_access_applications()
conditionsapplications.IncludeApplications(['All', ])


conditions.applications = conditionsapplications
conditionsusers = Conditional_access_users()
conditionsusers.IncludeUsers(['4628e7df-dff3-407c-a08f-75f08c0806dc', ])


conditions.users = conditionsusers

request_body.conditions = conditions
grant_controls = Conditional_access_grant_controls()
grant_controls.operator = 'OR'

grant_controls.BuiltInControls([grant_controls.conditionalaccessgrantcontrol(ConditionalAccessGrantControl.Mfa('conditionalaccessgrantcontrol.mfa'))
])


request_body.grant_controls = grant_controls



result = await client.identity.conditional_access.policies.post(request_body = request_body)


```