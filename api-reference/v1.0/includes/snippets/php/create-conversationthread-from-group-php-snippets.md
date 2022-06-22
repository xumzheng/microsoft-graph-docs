---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationThread();


$requestRequestBody->setTopic('New Conversation Thread Topic');
$postsArray = [];

$posts1 = new Post();


$body = new ItemBody();
$posts1->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('this is body content');

$newParticipantsArray = [];

$newParticipants1 = new Recipient();

$newParticipants1AdditionalData = [
	];
$newParticipants1->setAdditionalData($newParticipants1AdditionalData);

$newParticipantsArray []= $newParticipants1;
$posts1->setNewParticipants($newParticipantsArray);

$postsArray []= $posts1;
$requestRequestBody->setPosts($postsArray);
$result =  $graphClient->groupsById('group-id')->threads()->post($requestRequestBody);


```