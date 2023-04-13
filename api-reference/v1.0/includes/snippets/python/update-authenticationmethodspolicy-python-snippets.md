---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationMethodsPolicy()
registration_enforcement = RegistrationEnforcement()
registration_enforcement_authentication_methods_registration_campaign = AuthenticationMethodsRegistrationCampaign()
registrationEnforcementAuthenticationMethodsRegistrationCampaign.snooze_duration_in_days = 1

registrationEnforcementAuthenticationMethodsRegistrationCampaign.State(AdvancedConfigState('enabled'))

registrationEnforcementAuthenticationMethodsRegistrationCampaign.ExcludeTargets([])

include_targets_authentication_methods_registration_campaign_include_target1 = AuthenticationMethodsRegistrationCampaignIncludeTarget()
includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.id = '3ee3a9de-0a86-4e12-a287-9769accf1ba2'

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.TargetType(AuthenticationMethodTargetType('group'))

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.targetedAuthenticationMethod = 'microsoftAuthenticator'


includeTargetsArray []= includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1;
registrationEnforcementAuthenticationMethodsRegistrationCampaign.includetargets(includeTargetsArray)



registrationEnforcement.authentication_methods_registration_campaign = registrationEnforcementAuthenticationMethodsRegistrationCampaign

request_body.registration_enforcement = registrationEnforcement



result = await client.policies.authenticationMethodsPolicy.patch(request_body = request_body)


```