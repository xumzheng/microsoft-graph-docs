---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Attachment();
requestBody.set@odatatype('#Microsoft.OutlookServices.ItemAttachment');

requestBody.setName('name-value');

additionalData = [
'item' => requestBody = Item();
		requestBody.set@odatatype('microsoft.graph.message');


requestBody.setItem($item);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.me().eventsById('event-id').attachments().post(requestBody);


```