---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Conversation();


$requestRequestBody->setTopic('New head count');
$threadsArray = [];

$threads1 = new ConversationThread();

$postsArray = [];

$posts1 = new Post();


$body = new ItemBody();
$posts1->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('The confirmation will come by the end of the week.');

$newParticipantsArray = [];

$newParticipants1 = new Recipient();

$newParticipants1AdditionalData = [
		];
$newParticipants1->setAdditionalData($newParticipants1AdditionalData);

$newParticipantsArray []= $newParticipants1;
$posts1->setNewParticipants($newParticipantsArray);

$postsArray []= $posts1;
$threads1->setPosts($postsArray);

$threadsArray []= $threads1;
$requestRequestBody->setThreads($threadsArray);
$result =  $graphClient->groupsById('group-id')->conversations()->post($requestRequestBody);


```