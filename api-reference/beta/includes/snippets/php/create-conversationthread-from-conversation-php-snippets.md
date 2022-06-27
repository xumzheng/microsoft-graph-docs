---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationThread();


$requestRequestBody->setTopic('Take your wellness days and rest');
$postsArray = [];

$postsposts1 = new Post();


$body = new ItemBody();
$postsposts1->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('Waiting for the summer holidays.');


$postsArray []= $postsposts1;
$requestRequestBody->setPosts($postsArray);
$result =  $graphClient->groupsById('group-id')->conversationsById('conversation-id')->threads()->post($requestRequestBody);


```