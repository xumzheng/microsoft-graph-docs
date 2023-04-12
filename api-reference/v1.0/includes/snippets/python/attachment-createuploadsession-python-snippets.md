---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateUploadSessionPostRequestBody()
attachmentItem = AttachmentItem()
attachmentItem.AttachmentType(AttachmentType('file'))

attachmentItem.name = 'flower'

attachmentItem.size = 3483322


request_body.attachmentItem = attachmentItem



result = await client.me.messages_by_id('message-id').attachments.createUploadSession.post(request_body = request_body)


```