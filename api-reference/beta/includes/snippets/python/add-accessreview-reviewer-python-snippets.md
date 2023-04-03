---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessReviewReviewer();
requestBody.setId('006111db-0810-4494-a6df-904d368bd81b');



requestResult = graphServiceClient.accessReviewsById('accessReview-id').reviewers().post(requestBody);


```