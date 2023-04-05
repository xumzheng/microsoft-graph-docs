---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.set@odatatype('#microsoft.graph.fileAttachment')

request_body.setName('smile')

additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
request_body.setAdditionalData(additionalData)




result = await client.me.messages._by_id('message-id').attachments.post(request_body)


```