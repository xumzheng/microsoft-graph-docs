---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Conditional_access_policy()
request_body.display_name = 'Require MFA to EXO from non-complaint devices.'

request_body.state(ConditionalAccessPolicyState.Enabled('conditionalaccesspolicystate.enabled'))

conditions = Conditional_access_condition_set()
conditionsapplications = Conditional_access_applications()
conditionsapplications.IncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ])


conditions.applications = conditionsapplications
conditionsusers = Conditional_access_users()
conditionsusers.IncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ])


conditions.users = conditionsusers
conditionsdevices = Conditional_access_devices()
conditionsdevices.IncludeDevices(['All', ])

conditionsdevices.ExcludeDevices(['Compliant', ])


conditions.devices = conditionsdevices

request_body.conditions = conditions
grant_controls = Conditional_access_grant_controls()
grant_controls.operator = 'OR'

grant_controls.BuiltInControls([grant_controls.conditionalaccessgrantcontrol(ConditionalAccessGrantControl.Mfa('conditionalaccessgrantcontrol.mfa'))
])


request_body.grant_controls = grant_controls



result = await client.identity.conditional_access.policies.post(request_body = request_body)


```