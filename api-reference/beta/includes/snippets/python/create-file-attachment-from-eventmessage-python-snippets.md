---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Attachment()
request_body.set@odatatype('#Microsoft.OutlookServices.FileAttachment')

request_body.setName('name-value')

request_body.setContentType('contentType-value')

request_body.setIsInline(false)

additionalData = [
'contentLocation' => 'contentLocation-value', 
'contentBytes' => 'contentBytes-value', 
];
request_body.setAdditionalData(additionalData)




result = await client.me_messagesby_id('message-id')_attachments.post(request_body)


```