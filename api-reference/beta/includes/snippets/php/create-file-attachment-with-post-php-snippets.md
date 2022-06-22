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
$body->setContent('Which quarter does that file cover? See my attachment.');

$attachmentsArray = [];

$attachments1 = new Attachment();

$attachments1->setName('Another file as attachment');
$attachments1AdditionalData = [
	"@odata.type" => '#microsoft.graph.fileAttachment',
	"contentBytes" => 'VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu',
];
$attachments1->setAdditionalData($attachments1AdditionalData);

$attachmentsArray []= $attachments1;
$post->setAttachments($attachmentsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->reply()->post($requestRequestBody);


```