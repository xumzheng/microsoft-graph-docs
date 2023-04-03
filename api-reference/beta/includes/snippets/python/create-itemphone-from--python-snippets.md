---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ItemPhone();
requestBody.setDisplayName('Car Phone');

requestBody.setNumber('+7 499 342 22 13');



result = awaitclient.me().profile().phones().post(requestBody);


```