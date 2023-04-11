---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodsPolicy()
registrationEnforcement = RegistrationEnforcement()
registrationEnforcementAuthenticationMethodsRegistrationCampaign = AuthenticationMethodsRegistrationCampaign()
registrationEnforcementAuthenticationMethodsRegistrationCampaign.snoozeDurationInDays = 1

registrationEnforcementAuthenticationMethodsRegistrationCampaign.State(AdvancedConfigState('enabled'))

registrationEnforcementAuthenticationMethodsRegistrationCampaign.ExcludeTargets([])

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1 = AuthenticationMethodsRegistrationCampaignIncludeTarget()
includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.id = '3ee3a9de-0a86-4e12-a287-9769accf1ba2'

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.TargetType(AuthenticationMethodTargetType('group'))

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.targetedAuthenticationMethod = 'microsoftAuthenticator'


includeTargetsArray []= includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1;
registrationEnforcementAuthenticationMethodsRegistrationCampaign.includetargets(includeTargetsArray)



registrationEnforcement.authenticationMethodsRegistrationCampaign = registrationEnforcementAuthenticationMethodsRegistrationCampaign

request_body.registrationEnforcement = registrationEnforcement


request_configuration = AuthenticationMethodsPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.authenticationMethodsPolicy.patch(request_body = request_body)


```