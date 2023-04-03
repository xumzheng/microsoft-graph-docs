---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Subscription();
requestBody.setExpirationDateTime(DateTime('2016-03-22T11:00:00.0000000Z'));



result = awaitclient.subscriptionsById('subscription-id').patch(requestBody);


```