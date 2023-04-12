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



result = await client.me.events_by_id('event-id').attachments.createUploadSession.post(request_body = request_body)


```