---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Attachment();
requestBody.set@odatatype('#microsoft.graph.fileAttachment');

requestBody.setName('smile');

additionalData = [
'contentBytes' => 'a0b1c76de9f7=', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().messagesById('message-id').attachments().post(requestBody);


```