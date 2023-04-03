---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Attachment();
requestBody.set@odatatype('#Microsoft.OutlookServices.FileAttachment');

requestBody.setName('name-value');

requestBody.setContentType('contentType-value');

requestBody.setIsInline(false);

additionalData = [
'contentLocation' => 'contentLocation-value', 
'contentBytes' => 'contentBytes-value', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.me().messagesById('message-id').attachments().post(requestBody);


```