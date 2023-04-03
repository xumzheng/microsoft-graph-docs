---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CreateUploadSessionPostRequestBody();
attachmentItem = AttachmentItem();
attachmentItem.setAttachmentType(AttachmentType('file'));

attachmentItem.setName('flower');

attachmentItem.setSize(3483322);


requestBody.setAttachmentItem($attachmentItem);


result = await client.me().messagesById('message-id').attachments().createUploadSession().post(requestBody);


```