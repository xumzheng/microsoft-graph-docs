---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TeamworkTag();


$requestRequestBody->setDisplayName('Finance');
$membersArray = [];

$membersmembers1 = new TeamworkTagMember();

$membersmembers1->setUserId('92f6952f-61ca-4a94-8910-508a240bc167');

$membersArray []= $membersmembers1;

$membersmembers2 = new TeamworkTagMember();

$membersmembers2->setUserId('085d800c-b86b-4bfc-a857-9371ad1caf29');

$membersArray []= $membersmembers2;
$requestRequestBody->setMembers($membersArray);
$result =  $graphClient->teamsById('team-id')->tags()->post($requestRequestBody);


```