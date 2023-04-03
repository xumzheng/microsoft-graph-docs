---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonInterest();
requestBody.setCategories(['Sports', ]);



result = awaitclient.me().profile().interestsById('personInterest-id').patch(requestBody);


```