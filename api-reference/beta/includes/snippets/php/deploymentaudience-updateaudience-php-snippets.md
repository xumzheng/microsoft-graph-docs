---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdateAudiencePostRequestBody();


$addMembersArray = [];

$addMembersaddMembers1 = new UpdatableAsset();

$addMembersaddMembers1AdditionalData = [
	"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
	"id" => 'String (identifier)',
];
$addMembersaddMembers1->setAdditionalData($addMembersaddMembers1AdditionalData);

$addMembersArray []= $addMembersaddMembers1;
$requestRequestBody->setAddMembers($addMembersArray);
$removeMembersArray = [];

$removeMembersremoveMembers1 = new UpdatableAsset();

$removeMembersremoveMembers1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
"id" => 'String (identifier)',
];
$removeMembersremoveMembers1->setAdditionalData($removeMembersremoveMembers1AdditionalData);

$removeMembersArray []= $removeMembersremoveMembers1;
$requestRequestBody->setRemoveMembers($removeMembersArray);
$addExclusionsArray = [];

$addExclusionsaddExclusions1 = new UpdatableAsset();

$addExclusionsaddExclusions1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
"id" => 'String (identifier)',
];
$addExclusionsaddExclusions1->setAdditionalData($addExclusionsaddExclusions1AdditionalData);

$addExclusionsArray []= $addExclusionsaddExclusions1;
$requestRequestBody->setAddExclusions($addExclusionsArray);
$removeExclusionsArray = [];

$removeExclusionsremoveExclusions1 = new UpdatableAsset();

$removeExclusionsremoveExclusions1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
"id" => 'String (identifier)',
];
$removeExclusionsremoveExclusions1->setAdditionalData($removeExclusionsremoveExclusions1AdditionalData);

$removeExclusionsArray []= $removeExclusionsremoveExclusions1;
$requestRequestBody->setRemoveExclusions($removeExclusionsArray);
$result =  $graphClient->admin()->windows()->updates()->deploymentsById('deployment-id')->audience()->updateAudience()->post($requestRequestBody);


```