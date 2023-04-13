---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.displayName = 'Access to EXO requires MFA'

request_body.State(ConditionalAccessPolicyState('enabled'))

conditions = ConditionalAccessConditionSet()
conditions.ClientAppTypes([conditions.ConditionalAccessClientApp(ConditionalAccessClientApp('mobileappsanddesktopclients'))
conditions.ConditionalAccessClientApp(ConditionalAccessClientApp('browser'))
])

conditions_applications = ConditionalAccessApplications()
conditionsApplications.IncludeApplications(['00000002-0000-0ff1-ce00-000000000000', ])


conditions.applications = conditionsApplications
conditions_users = ConditionalAccessUsers()
conditionsUsers.IncludeGroups(['ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba', ])


conditions.users = conditionsUsers
conditions_locations = ConditionalAccessLocations()
conditionsLocations.IncludeLocations(['All', ])

conditionsLocations.ExcludeLocations(['AllTrusted', ])


conditions.locations = conditionsLocations

request_body.conditions = conditions
grant_controls = ConditionalAccessGrantControls()
grantControls.operator = 'OR'

grantControls.BuiltInControls([grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'))
])


request_body.grant_controls = grantControls



result = await client.identity.conditionalAccess.policies.post(request_body = request_body)


```