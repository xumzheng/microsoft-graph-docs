---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CreateReplyAllPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$attachmentsArray = [];

$attachments1 = new Attachment();

$attachments1->setName('guidelines.txt');
$attachments1AdditionalData = [
		"@odata.type" => '#microsoft.graph.fileAttachment',
		"contentBytes" => 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=',
	];
$attachments1->setAdditionalData($attachments1AdditionalData);

$attachmentsArray []= $attachments1;
$message->setAttachments($attachmentsArray);

$requestRequestBody->setComment('if the project gets approved, please take a look at the attached guidelines before you decide on the name.');
$result =  $graphClient->me()->messagesById('message-id')->createReplyAll()->post($requestRequestBody);


```