---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DismissPostRequestBody();
requestBody.setDismissReason('Recommendations is not relevant for my organization because...');



result = awaitclient.directory().recommendationsById('recommendation-id').dismiss().post(requestBody);


```