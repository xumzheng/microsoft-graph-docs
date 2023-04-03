---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Attachment();
requestBody.set@odatatype('#microsoft.graph.itemAttachment');

requestBody.setName('Holiday event');

additionalData = [
'item' => requestBody = Item();
		requestBody.set@odatatype('microsoft.graph.event');

		requestBody.setSubject('Discuss gifts for children');

body = Body();
		body.setContentType('HTML');

		body.setContent('Let\'s look for funding!');


requestBody.setBody($body);
start = Start();
		start.setDateTime('2016-12-02T18:00:00');

		start.setTimeZone('Pacific Standard Time');


requestBody.setStart($start);
end = End();
		end.setDateTime('2016-12-02T19:00:00');

		end.setTimeZone('Pacific Standard Time');


requestBody.setEnd($end);

requestBody.setItem($item);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.me().eventsById('event-id').attachments().post(requestBody);


```