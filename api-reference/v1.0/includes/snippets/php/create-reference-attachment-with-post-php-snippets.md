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
$body->setContent('I attached a reference to a file on OneDrive.');

$attachmentsArray = [];

$attachments1 = new Attachment();

$attachments1->setName('Personal pictures');
$attachments1AdditionalData = [
	"@odata.type" => '#microsoft.graph.referenceAttachment',
	"sourceUrl" => 'https://contoso.com/personal/mario_contoso_net/Documents/Pics',
	"providerType" => 'oneDriveConsumer',
	"permission" => 'Edit',
	"isFolder" => 'True',
];
$attachments1->setAdditionalData($attachments1AdditionalData);

$attachmentsArray []= $attachments1;
$post->setAttachments($attachmentsArray);

$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->reply()->post($requestRequestBody);


```