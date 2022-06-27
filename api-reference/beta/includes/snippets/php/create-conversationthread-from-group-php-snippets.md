---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationThread();


$requestRequestBody->setTopic('New Conversation Thread Topic');
$postsArray = [];

$postsposts1 = new Post();


$body = new ItemBody();
$postsposts1->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('this is body content');

$newParticipantsArray = [];

$newParticipantsnewParticipants1 = new Recipient();

$newParticipantsnewParticipants1AdditionalData = [
];
$newParticipantsnewParticipants1->setAdditionalData($newParticipantsnewParticipants1AdditionalData);

$newParticipantsArray []= $newParticipantsnewParticipants1;
$postsposts1->setNewParticipants($newParticipantsArray);

$postsArray []= $postsposts1;
$requestRequestBody->setPosts($postsArray);
$result =  $graphClient->groupsById('group-id')->threads()->post($requestRequestBody);


```