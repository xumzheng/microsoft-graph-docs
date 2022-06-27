---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AttachmentItemRequestBody();



$attachmentItem = new AttachmentItem();
$requestRequestBody->setAttachmentItem($attachmentItem);


$attachmentItem->setAttachmentType(new AttachmentType('file'));
$attachmentItem->setName('scenary');
$attachmentItem->setSize(7208534);
$attachmentItem->setIsInline(True);
$attachmentItem->setContentId('my_inline_picture');

$result =  $graphClient->me()->messagesById('message-id')->attachments()->createUploadSession()->post($requestRequestBody);


```