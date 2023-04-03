---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonInterest();
requestBody.setCategories(['Sports', ]);



result = await client.me().profile().interestsById('personInterest-id').patch(requestBody);


```