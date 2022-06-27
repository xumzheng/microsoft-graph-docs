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

$includeTargetsincludeTargets1 = new AuthenticationMethodsRegistrationCampaignIncludeTarget();

$includeTargetsincludeTargets1AdditionalData = [
"id" => '3ee3a9de-0a86-4e12-a287-9769accf1ba2',
"targetType" => 'group',
"targetedAuthenticationMethod" => 'microsoftAuthenticator',
];
$includeTargetsincludeTargets1->setAdditionalData($includeTargetsincludeTargets1AdditionalData);

$includeTargetsArray []= $includeTargetsincludeTargets1;
$authenticationMethodsRegistrationCampaign->setIncludeTargets($includeTargetsArray);


$result =  $graphClient->policies()->authenticationMethodsPolicy()->patch($requestRequestBody);


```