---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CreateUploadSessionPostRequestBody();
attachmentItem = AttachmentItem();
attachmentItem.setAttachmentType(AttachmentType('file'));

attachmentItem.setName('scenary');

attachmentItem.setSize(7208534);

attachmentItem.setIsInline(true);

attachmentItem.setContentId('my_inline_picture');


request_body.setAttachmentItem($attachmentItem);


result = await client.me().messagesById('message-id').attachments().createUploadSession().post(request_body);


```