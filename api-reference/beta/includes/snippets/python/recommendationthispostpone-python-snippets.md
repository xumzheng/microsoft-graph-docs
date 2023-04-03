---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PostponePostRequestBody();
requestBody.setPostponeUntilDateTime(DateTime('2023-02-01T02:53:00Z'));



result = awaitclient.directory().recommendationsById('recommendation-id').postpone().post(requestBody);


```