---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CreateUploadSessionPostRequestBody();
attachmentItem = AttachmentItem();
attachmentItem.setAttachmentType(AttachmentType('file'));

attachmentItem.setName('flower');

attachmentItem.setSize(3483322);


requestBody.setAttachmentItem($attachmentItem);


requestResult = graphServiceClient.me().eventsById('event-id').attachments().createUploadSession().post(requestBody);


```