---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GovernanceRoleSetting();


$adminEligibleSettingsArray = [];

$adminEligibleSettingsadminEligibleSettings1 = new GovernanceRuleSetting();

$adminEligibleSettingsadminEligibleSettings1->setRuleIdentifier('ExpirationRule');
$adminEligibleSettingsadminEligibleSettings1->setSetting('{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}');

$adminEligibleSettingsArray []= $adminEligibleSettingsadminEligibleSettings1;
$requestRequestBody->setAdminEligibleSettings($adminEligibleSettingsArray);
$result =  $graphClient->privilegedAccessById('privilegedAccess-id')->roleSettingsById('governanceRoleSetting-id')->patch($requestRequestBody);


```