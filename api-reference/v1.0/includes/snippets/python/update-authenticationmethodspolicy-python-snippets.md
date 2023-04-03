---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthenticationMethodsPolicy();
registrationEnforcement = RegistrationEnforcement();
registrationEnforcementAuthenticationMethodsRegistrationCampaign = AuthenticationMethodsRegistrationCampaign();
registrationEnforcementAuthenticationMethodsRegistrationCampaign.setSnoozeDurationInDays(1);

registrationEnforcementAuthenticationMethodsRegistrationCampaign.setState(AdvancedConfigState('enabled'));

registrationEnforcementAuthenticationMethodsRegistrationCampaign.setExcludeTargets([]);

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1 = AuthenticationMethodsRegistrationCampaignIncludeTarget();
includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.setId('3ee3a9de-0a86-4e12-a287-9769accf1ba2');

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.setTargetType(AuthenticationMethodTargetType('group'));

includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1.setTargetedAuthenticationMethod('microsoftAuthenticator');


includeTargetsArray []= includeTargetsAuthenticationMethodsRegistrationCampaignIncludeTarget1;
registrationEnforcementAuthenticationMethodsRegistrationCampaign.setIncludeTargets(includeTargetsArray);



registrationEnforcement.setAuthenticationMethodsRegistrationCampaign($registrationEnforcementAuthenticationMethodsRegistrationCampaign);

requestBody.setRegistrationEnforcement($registrationEnforcement);


requestResult = graphServiceClient.policies().authenticationMethodsPolicy().patch(requestBody);


```