---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessReview();
requestBody.setDisplayName('TestReview new name');



result = await client.accessReviewsById('accessReview-id').patch(requestBody);


```