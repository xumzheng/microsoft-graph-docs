---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleSetting();


$adminEligibleSettingsArray = [];

$adminEligibleSettings1 = new GovernanceRuleSetting();

$adminEligibleSettings1->setRuleIdentifier('ExpirationRule');
$adminEligibleSettings1->setSetting('{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}');

$adminEligibleSettingsArray []= $adminEligibleSettings1;
$requestRequestBody->setAdminEligibleSettings($adminEligibleSettingsArray);
$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleSettingsById('governanceRoleSetting-id')->patch($requestRequestBody);


```