---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdateAudiencePostRequestBody();


$addMembersArray = [];

$addMembers1 = new UpdatableAsset();

$addMembers1AdditionalData = [
		"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
		"id" => 'String (identifier)',
	];
$addMembers1->setAdditionalData($addMembers1AdditionalData);

$addMembersArray []= $addMembers1;
$requestRequestBody->setAddMembers($addMembersArray);
$removeMembersArray = [];

$removeMembers1 = new UpdatableAsset();

$removeMembers1AdditionalData = [
	"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
	"id" => 'String (identifier)',
];
$removeMembers1->setAdditionalData($removeMembers1AdditionalData);

$removeMembersArray []= $removeMembers1;
$requestRequestBody->setRemoveMembers($removeMembersArray);
$addExclusionsArray = [];

$addExclusions1 = new UpdatableAsset();

$addExclusions1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
"id" => 'String (identifier)',
];
$addExclusions1->setAdditionalData($addExclusions1AdditionalData);

$addExclusionsArray []= $addExclusions1;
$requestRequestBody->setAddExclusions($addExclusionsArray);
$removeExclusionsArray = [];

$removeExclusions1 = new UpdatableAsset();

$removeExclusions1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
"id" => 'String (identifier)',
];
$removeExclusions1->setAdditionalData($removeExclusions1AdditionalData);

$removeExclusionsArray []= $removeExclusions1;
$requestRequestBody->setRemoveExclusions($removeExclusionsArray);
$result =  $graphClient->admin()->windows()->updates()->deploymentsById('deployment-id')->audience()->updateAudience()->post($requestRequestBody);


```