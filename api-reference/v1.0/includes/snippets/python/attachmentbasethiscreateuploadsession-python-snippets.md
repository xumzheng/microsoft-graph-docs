---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateUploadSessionPostRequestBody()
attachmentInfo = AttachmentInfo()
attachmentInfo.setAttachmentType(AttachmentType('file'))

attachmentInfo.setName('flower')

attachmentInfo.setSize(3483322)


request_body.setAttachmentInfo($attachmentInfo)


result = await client.me.todo.lists._by_id('todoTaskList-id').tasks._by_id('todoTask-id').attachments.createUploadSession.post(request_body)


```