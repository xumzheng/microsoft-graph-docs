---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Attachment();
request_body.set@odatatype('microsoft.graph.fileAttachment');

request_body.setName('name-value');

request_body.setContentType('contentType-value');

request_body.setIsInline(false);

additionalData = [
'contentLocation' => 'contentLocation-value', 
'contentBytes' => 'base64-contentBytes-value', 
];
request_body.setAdditionalData(additionalData);




result = await client.me().messagesById('message-id').attachments().post(request_body);


```