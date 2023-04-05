---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.set@odatatype('#microsoft.graph.fileAttachment')

request_body.setName('menu.txt')

additionalData = [
'contentBytes' => 'base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=', 
];
request_body.setAdditionalData(additionalData)




result = await client.me.eventsby_id('event-id').attachments.post(request_body)


```