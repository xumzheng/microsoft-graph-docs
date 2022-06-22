---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConditionalAccessPolicy();


$requestRequestBody->setDisplayName('Access to EXO requires MFA');
$requestRequestBody->setState(new ConditionalAccessPolicyState('enabled'));

$conditions = new ConditionalAccessConditionSet();
$requestRequestBody->setConditions($conditions);


$clientAppTypesArray = [];
'mobileAppsAndDesktopClients',$clientAppTypesArray []= $clientAppTypes1;
'browser',$clientAppTypesArray []= $clientAppTypes2;
$conditions->setClientAppTypes($clientAppTypesArray);

$applications = new ConditionalAccessApplications();
$conditions->setApplications($applications);


$applications->setIncludeApplications( [
'00000002-0000-0ff1-ce00-000000000000',],


$users = new ConditionalAccessUsers();
$conditions->setUsers($users);


$users->setIncludeGroups( [
'ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba',],


$locations = new ConditionalAccessLocations();
$conditions->setLocations($locations);


$locations->setIncludeLocations( [
'All',],
$locations->setExcludeLocations( [
'AllTrusted',],



$grantControls = new ConditionalAccessGrantControls();
$requestRequestBody->setGrantControls($grantControls);


$grantControls->setOperator('OR');
$builtInControlsArray = [];
'mfa',$builtInControlsArray []= $builtInControls1;
$grantControls->setBuiltInControls($builtInControlsArray);

$result =  $graphClient->identity()->conditionalAccess()->policies()->post($requestRequestBody);


```