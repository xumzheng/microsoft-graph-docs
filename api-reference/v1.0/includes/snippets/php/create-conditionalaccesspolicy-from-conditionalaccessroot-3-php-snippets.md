---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConditionalAccessPolicy();


$requestRequestBody->setDisplayName('Demo app for documentation');
$requestRequestBody->setState(new ConditionalAccessPolicyState('disabled'));

$conditions = new ConditionalAccessConditionSet();
$requestRequestBody->setConditions($conditions);


$signInRiskLevelsArray = [];
'high',$signInRiskLevelsArray []= $signInRiskLevels1;
'medium',$signInRiskLevelsArray []= $signInRiskLevels2;
$conditions->setSignInRiskLevels($signInRiskLevelsArray);
$clientAppTypesArray = [];
'mobileAppsAndDesktopClients',$clientAppTypesArray []= $clientAppTypes1;
'exchangeActiveSync',$clientAppTypesArray []= $clientAppTypes2;
'other',$clientAppTypesArray []= $clientAppTypes3;
$conditions->setClientAppTypes($clientAppTypesArray);

$applications = new ConditionalAccessApplications();
$conditions->setApplications($applications);


$applications->setIncludeApplications( [
'All',],
$applications->setExcludeApplications( [
'499b84ac-1321-427f-aa17-267ca6975798','00000007-0000-0000-c000-000000000000','de8bc8b5-d9f9-48b1-a8ad-b748da725064','00000012-0000-0000-c000-000000000000','797f4846-ba00-4fd7-ba43-dac1f8f63013','05a65629-4c1b-48c1-a78b-804c4abdd4af','7df0a125-d3be-4c96-aa54-591f83ff541c',],
$applications->setIncludeUserActions( [
],


$users = new ConditionalAccessUsers();
$conditions->setUsers($users);


$users->setIncludeUsers( [
'a702a13d-a437-4a07-8a7e-8c052de62dfd',],
$users->setExcludeUsers( [
'124c5b6a-ffa5-483a-9b88-04c3fce5574a','GuestsOrExternalUsers',],
$users->setIncludeGroups( [
],
$users->setExcludeGroups( [
],
$users->setIncludeRoles( [
'9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3','cf1c38e5-3621-4004-a7cb-879624dced7c','c4e39bd9-1100-46d3-8c65-fb160da0071f',],
$users->setExcludeRoles( [
'b0f54661-2d74-4c50-afa3-1ec803f12efe',],


$platforms = new ConditionalAccessPlatforms();
$conditions->setPlatforms($platforms);


$includePlatformsArray = [];
'all',$includePlatformsArray []= $includePlatforms1;
$platforms->setIncludePlatforms($includePlatformsArray);
$excludePlatformsArray = [];
'iOS',$excludePlatformsArray []= $excludePlatforms1;
'windowsPhone',$excludePlatformsArray []= $excludePlatforms2;
$platforms->setExcludePlatforms($excludePlatformsArray);


$locations = new ConditionalAccessLocations();
$conditions->setLocations($locations);


$locations->setIncludeLocations( [
'AllTrusted',],
$locations->setExcludeLocations( [
'00000000-0000-0000-0000-000000000000','d2136c9c-b049-47ae-b9cf-316e04ef7198',],



$grantControls = new ConditionalAccessGrantControls();
$requestRequestBody->setGrantControls($grantControls);


$grantControls->setOperator('OR');
$builtInControlsArray = [];
'mfa',$builtInControlsArray []= $builtInControls1;
'compliantDevice',$builtInControlsArray []= $builtInControls2;
'domainJoinedDevice',$builtInControlsArray []= $builtInControls3;
'approvedApplication',$builtInControlsArray []= $builtInControls4;
'compliantApplication',$builtInControlsArray []= $builtInControls5;
$grantControls->setBuiltInControls($builtInControlsArray);
$grantControls->setCustomAuthenticationFactors( [
],
$grantControls->setTermsOfUse( [
'ce580154-086a-40fd-91df-8a60abac81a0','7f29d675-caff-43e1-8a53-1b8516ed2075',],


$sessionControls = new ConditionalAccessSessionControls();
$requestRequestBody->setSessionControls($sessionControls);


$sessionControls->setApplicationEnforcedRestrictions(null);
$sessionControls->setPersistentBrowser(null);

$cloudAppSecurity = new CloudAppSecuritySessionControl();
$sessionControls->setCloudAppSecurity($cloudAppSecurity);


$cloudAppSecurity->setCloudAppSecurityType(new CloudAppSecuritySessionControlType('blockDownloads'));
$cloudAppSecurity->setIsEnabled(True);


$signInFrequency = new SignInFrequencySessionControl();
$sessionControls->setSignInFrequency($signInFrequency);


$signInFrequency->setValue(4);
$signInFrequency->setType(new SigninFrequencyType('hours'));
$signInFrequency->setIsEnabled(True);


$result =  $graphClient->identity()->conditionalAccess()->policies()->post($requestRequestBody);


```