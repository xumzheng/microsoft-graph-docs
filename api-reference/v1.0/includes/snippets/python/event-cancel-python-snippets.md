---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CancelPostRequestBody();
requestBody.setComment('Cancelling for this week due to all hands');



graphServiceClient.me().eventsById('event-id').cancel().post(requestBody);


```