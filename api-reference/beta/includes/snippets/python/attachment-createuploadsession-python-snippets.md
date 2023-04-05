---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateUploadSessionPostRequestBody()
attachmentItem = AttachmentItem()
attachmentItem.setAttachmentType(AttachmentType('file'))

attachmentItem.setName('flower')

attachmentItem.setSize(3483322)


request_body.setAttachmentItem($attachmentItem)


result = await client.me_messagesby_id('message-id')_attachments_createUploadSession.post(request_body)


```