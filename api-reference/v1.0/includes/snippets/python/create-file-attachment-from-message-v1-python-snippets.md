---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Attachment();
requestBody.set@odatatype('#microsoft.graph.fileAttachment');

requestBody.setName('smile');

additionalData = [
'contentBytes' => 'R0lGODdhEAYEAA7', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.me().messagesById('message-id').attachments().post(requestBody);


```