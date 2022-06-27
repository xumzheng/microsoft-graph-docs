---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationThread();


$requestRequestBodyAdditionalData = [
	"originalStartTimeZone" => 'originalStartTimeZone-value',
	"originalEndTimeZone" => 'originalEndTimeZone-value',
	"iCalUId" => 'iCalUId-value',
	"reminderMinutesBeforeStart" => 99,
	"isReminderOn" => True,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->patch($requestRequestBody);


```