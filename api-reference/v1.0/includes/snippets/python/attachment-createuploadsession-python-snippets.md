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



result = await client.me.messages_by_id('message-id').attachments.createUploadSession.post(request_body = request_body)


```