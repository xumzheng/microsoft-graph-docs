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


$result =  $graphClient->policies()->authenticationMethodsPolicy()->patch($requestRequestBody);


```