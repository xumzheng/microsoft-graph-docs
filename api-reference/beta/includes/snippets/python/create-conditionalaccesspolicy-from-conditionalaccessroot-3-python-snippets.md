---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy()
request_body.displayName = 'Demo app for documentation'

request_body.State(ConditionalAccessPolicyState('disabled'))

conditions = ConditionalAccessConditionSet()
conditions.SignInRiskLevels([conditions.RiskLevel(RiskLevel('high'))
conditions.RiskLevel(RiskLevel('medium'))
])

conditions.ClientAppTypes([conditions.ConditionalAccessClientApp(ConditionalAccessClientApp('mobileappsanddesktopclients'))
conditions.ConditionalAccessClientApp(ConditionalAccessClientApp('exchangeactivesync'))
conditions.ConditionalAccessClientApp(ConditionalAccessClientApp('other'))
])

conditions_applications = ConditionalAccessApplications()
conditionsApplications.IncludeApplications(['All', ])

conditionsApplications.ExcludeApplications(['499b84ac-1321-427f-aa17-267ca6975798', '00000007-0000-0000-c000-000000000000', 'de8bc8b5-d9f9-48b1-a8ad-b748da725064', '00000012-0000-0000-c000-000000000000', '797f4846-ba00-4fd7-ba43-dac1f8f63013', '05a65629-4c1b-48c1-a78b-804c4abdd4af', '7df0a125-d3be-4c96-aa54-591f83ff541c', ])

conditionsApplications.IncludeUserActions([])


conditions.applications = conditionsApplications
conditions_users = ConditionalAccessUsers()
conditionsUsers.IncludeUsers(['a702a13d-a437-4a07-8a7e-8c052de62dfd', ])

conditionsUsers.ExcludeUsers(['124c5b6a-ffa5-483a-9b88-04c3fce5574a', 'GuestsOrExternalUsers', ])

conditionsUsers.IncludeGroups([])

conditionsUsers.ExcludeGroups([])

conditionsUsers.IncludeRoles(['9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3', 'cf1c38e5-3621-4004-a7cb-879624dced7c', 'c4e39bd9-1100-46d3-8c65-fb160da0071f', ])

conditionsUsers.ExcludeRoles(['b0f54661-2d74-4c50-afa3-1ec803f12efe', ])


conditions.users = conditionsUsers
conditions_platforms = ConditionalAccessPlatforms()
conditionsPlatforms.IncludePlatforms([conditionsPlatforms.ConditionalAccessDevicePlatform(ConditionalAccessDevicePlatform('all'))
])

conditionsPlatforms.ExcludePlatforms([conditionsPlatforms.ConditionalAccessDevicePlatform(ConditionalAccessDevicePlatform('ios'))
conditionsPlatforms.ConditionalAccessDevicePlatform(ConditionalAccessDevicePlatform('windowsphone'))
])


conditions.platforms = conditionsPlatforms
conditions_locations = ConditionalAccessLocations()
conditionsLocations.IncludeLocations(['AllTrusted', ])

conditionsLocations.ExcludeLocations(['00000000-0000-0000-0000-000000000000', 'd2136c9c-b049-47ae-b9cf-316e04ef7198', ])


conditions.locations = conditionsLocations
conditions_device_states = ConditionalAccessDeviceStates()
conditionsDeviceStates.IncludeStates(['All', ])

conditionsDeviceStates.ExcludeStates(['Compliant', ])


conditions.device_states = conditionsDeviceStates

request_body.conditions = conditions
grant_controls = ConditionalAccessGrantControls()
grantControls.operator = 'OR'

grantControls.BuiltInControls([grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('mfa'))
grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('compliantdevice'))
grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('domainjoineddevice'))
grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('approvedapplication'))
grantControls.ConditionalAccessGrantControl(ConditionalAccessGrantControl('compliantapplication'))
])

grantControls.CustomAuthenticationFactors([])

grantControls.TermsOfUse(['ce580154-086a-40fd-91df-8a60abac81a0', '7f29d675-caff-43e1-8a53-1b8516ed2075', ])


request_body.grant_controls = grantControls
session_controls = ConditionalAccessSessionControls()
SessionControls.applicationEnforcedRestrictions=null

SessionControls.persistentBrowser=null

session_controls_cloud_app_security = CloudAppSecuritySessionControl()
sessionControlsCloudAppSecurity.CloudAppSecurityType(CloudAppSecuritySessionControlType('blockdownloads'))

sessionControlsCloudAppSecurity.is_enabled = True


sessionControls.cloud_app_security = sessionControlsCloudAppSecurity
session_controls_sign_in_frequency = SignInFrequencySessionControl()
sessionControlsSignInFrequency.value = 4

sessionControlsSignInFrequency.Type(SigninFrequencyType('hours'))

sessionControlsSignInFrequency.is_enabled = True


sessionControls.sign_in_frequency = sessionControlsSignInFrequency

request_body.session_controls = sessionControls



result = await client.identity.conditionalAccess.policies.post(request_body = request_body)


```