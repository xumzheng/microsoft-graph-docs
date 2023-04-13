---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Message()
request_body.receivedDateTime = DateTime('datetime-value')

request_body.sentDateTime = DateTime('datetime-value')

request_body.has_attachments = True

request_body.subject = 'subject-value'

body = ItemBody()
body.ContentType(BodyType('text'))

body.content = 'content-value'


request_body.body = body
request_body.bodyPreview = 'bodyPreview-value'




result = await client.me.mailFolders_by_id('mailFolder-id').messages.post(request_body = request_body)


```