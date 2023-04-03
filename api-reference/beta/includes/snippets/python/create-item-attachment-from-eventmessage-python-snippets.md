---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Attachment();
requestBody.set@odatatype('#Microsoft.OutlookServices.ItemAttachment');

requestBody.setName('name-value');

additionalData = [
'item' => requestBody = Item();
		requestBody.set@odatatype('microsoft.graph.message');


requestBody.setItem($item);

];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.me().eventsById('event-id').attachments().post(requestBody);


```