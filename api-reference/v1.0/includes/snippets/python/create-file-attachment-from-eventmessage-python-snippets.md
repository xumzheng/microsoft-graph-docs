---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.@odatatype = 'microsoft.graph.fileAttachment'

request_body.name = 'name-value'

request_body.contentType = 'contentType-value'

request_body.is_inline = False

additionalData = [
'contentLocation' => 'contentLocation-value', 
'contentBytes' => 'base64-contentBytes-value', 
];
request_body.additionaldata(additionalData)





result = await client.me.messages_by_id('message-id').attachments.post(request_body = request_body)


```