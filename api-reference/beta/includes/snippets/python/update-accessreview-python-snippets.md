---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessReview();
requestBody.setDisplayName('TestReview new name');



requestResult = graphServiceClient.accessReviewsById('accessReview-id').patch(requestBody);


```