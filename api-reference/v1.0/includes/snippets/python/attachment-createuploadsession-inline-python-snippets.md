---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CreateUploadSessionPostRequestBody();
$attachmentItem = new AttachmentItem();
$attachmentItem.setAttachmentType(new AttachmentType('file'));

$attachmentItem.setName('scenary');

$attachmentItem.setSize(7208534);

$attachmentItem.setIsInline(true);

$attachmentItem.setContentId('my_inline_picture');


$requestBody.setAttachmentItem($attachmentItem);


$requestResult = $graphServiceClient.me().messagesById('message-id').attachments().createUploadSession().post($requestBody);


```