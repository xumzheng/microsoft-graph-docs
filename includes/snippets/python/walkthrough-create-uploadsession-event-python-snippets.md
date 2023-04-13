---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateUploadSessionPostRequestBody()
attachment_item = AttachmentItem()
attachmentItem.AttachmentType(AttachmentType('file'))

attachmentItem.name = 'flower'

attachmentItem.size = 3483322


request_body.attachment_item = attachmentItem



result = await client.me.events_by_id('event-id').attachments.createUploadSession.post(request_body = request_body)


```