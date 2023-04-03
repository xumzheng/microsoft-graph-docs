---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessReview();
requestBody.setDisplayName('TestReview new name');



result = awaitclient.accessReviewsById('accessReview-id').patch(requestBody);


```