---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Conversation();


$requestRequestBody->setTopic('Take your wellness days and rest');
$threadsArray = [];

$threadsthreads1 = new ConversationThread();

$postsArray = [];

$postsposts1 = new Post();


$body = new ItemBody();
$postsposts1->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('Contoso cares about you: Rest and Recharge');

$newParticipantsArray = [];

$newParticipantsnewParticipants1 = new Recipient();

$newParticipantsnewParticipants1AdditionalData = [
];
$newParticipantsnewParticipants1->setAdditionalData($newParticipantsnewParticipants1AdditionalData);

$newParticipantsArray []= $newParticipantsnewParticipants1;
$postsposts1->setNewParticipants($newParticipantsArray);

$postsArray []= $postsposts1;
$threadsthreads1->setPosts($postsArray);

$threadsArray []= $threadsthreads1;
$requestRequestBody->setThreads($threadsArray);
$result =  $graphClient->groupsById('group-id')->conversations()->post($requestRequestBody);


```