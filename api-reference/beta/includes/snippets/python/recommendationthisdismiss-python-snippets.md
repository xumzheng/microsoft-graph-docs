---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DismissPostRequestBody();
requestBody.setDismissReason('Recommendations is not relevant for my organization because...');



result = await client.directory().recommendationsById('recommendation-id').dismiss().post(requestBody);


```