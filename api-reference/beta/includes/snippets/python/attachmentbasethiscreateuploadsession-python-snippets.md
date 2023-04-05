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


result = await client.me_todo_listsby_id('todoTaskList-id')_tasksby_id('todoTask-id')_attachments_createUploadSession.post(request_body)


```