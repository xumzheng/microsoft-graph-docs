---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Subscription();
requestBody.setExpirationDateTime(DateTime('2016-11-22T18:23:45.9356913Z'));



requestResult = graphServiceClient.subscriptionsById('subscription-id').patch(requestBody);


```