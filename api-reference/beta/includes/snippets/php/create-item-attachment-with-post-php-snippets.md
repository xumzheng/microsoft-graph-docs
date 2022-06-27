---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PostRequestBody();



$post = new Post();
$requestRequestBody->setPost($post);



$body = new ItemBody();
$post->setBody($body);


$body->setContentType(new BodyType('text'));
$body->setContent('I attached an event.');

$attachmentsArray = [];

$attachmentsattachments1 = new Attachment();

$attachmentsattachments1->setName('Holiday event');
$attachmentsattachments1AdditionalData = [
"@odata.type" => '#microsoft.graph.itemAttachment',
];
$attachmentsattachments1->setAdditionalData($attachmentsattachments1AdditionalData);

$attachmentsArray []= $attachmentsattachments1;
$post->setAttachments($attachmentsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->reply()->post($requestRequestBody);


```