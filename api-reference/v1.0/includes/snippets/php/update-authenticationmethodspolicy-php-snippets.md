---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationMethodsPolicy();



$registrationEnforcement = new RegistrationEnforcement();
$requestRequestBody->setRegistrationEnforcement($registrationEnforcement);



$authenticationMethodsRegistrationCampaign = new AuthenticationMethodsRegistrationCampaign();
$registrationEnforcement->setAuthenticationMethodsRegistrationCampaign($authenticationMethodsRegistrationCampaign);


$authenticationMethodsRegistrationCampaign->setSnoozeDurationInDays(1);
$authenticationMethodsRegistrationCampaign->setState(new AdvancedConfigState('enabled'));
$excludeTargetsArray = [];
$authenticationMethodsRegistrationCampaign->setExcludeTargets($excludeTargetsArray);
$includeTargetsArray = [];

$includeTargets1 = new AuthenticationMethodsRegistrationCampaignIncludeTarget();

$includeTargets1AdditionalData = [
		"id" => '3ee3a9de-0a86-4e12-a287-9769accf1ba2',
		"targetType" => 'group',
		"targetedAuthenticationMethod" => 'microsoftAuthenticator',
	];
$includeTargets1->setAdditionalData($includeTargets1AdditionalData);

$includeTargetsArray []= $includeTargets1;
$authenticationMethodsRegistrationCampaign->setIncludeTargets($includeTargetsArray);


$authenticationMethodConfigurationsArray = [];

$authenticationMethodConfigurations1 = new AuthenticationMethodConfiguration();

$authenticationMethodConfigurations1->setId('Fido2');
$authenticationMethodConfigurations1->setState(new AuthenticationMethodState('disabled'));
$authenticationMethodConfigurations1AdditionalData = [
"@odata.type" => '#microsoft.graph.fido2AuthenticationMethodConfiguration',
"isSelfServiceRegistrationAllowed" => False,
"isAttestationEnforced" => False,
];
$authenticationMethodConfigurations1->setAdditionalData($authenticationMethodConfigurations1AdditionalData);

$authenticationMethodConfigurationsArray []= $authenticationMethodConfigurations1;
$requestRequestBody->setAuthenticationMethodConfigurations($authenticationMethodConfigurationsArray);
$requestRequestBodyAdditionalData = [
"@odata.context" => 'https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->authenticationMethodsPolicy()->patch($requestRequestBody);


```