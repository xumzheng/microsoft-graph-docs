---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Subscription();
requestBody.setExpirationDateTime(DateTime('2016-11-22T18:23:45.9356913Z'));



result = await client.subscriptionsById('subscription-id').patch(requestBody);


```