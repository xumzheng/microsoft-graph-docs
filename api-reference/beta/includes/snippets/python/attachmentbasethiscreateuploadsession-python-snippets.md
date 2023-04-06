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

request_config = CreateUploadSessionRequestBuilderPostRequestConfiguration(
request_config = CreateUploadSessionRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.todo.lists_by_id('todoTaskList-id').tasks_by_id('todoTask-id').attachments.createUploadSession.post(request_body, headers=)


```