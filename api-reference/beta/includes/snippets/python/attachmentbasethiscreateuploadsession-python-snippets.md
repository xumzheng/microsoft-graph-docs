---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CreateUploadSessionPostRequestBody();
attachmentInfo = AttachmentInfo();
attachmentInfo.setAttachmentType(AttachmentType('file'));

attachmentInfo.setName('flower');

attachmentInfo.setSize(3483322);


requestBody.setAttachmentInfo($attachmentInfo);


result = await client.me().todo().listsById('todoTaskList-id').tasksById('todoTask-id').attachments().createUploadSession().post(requestBody);


```