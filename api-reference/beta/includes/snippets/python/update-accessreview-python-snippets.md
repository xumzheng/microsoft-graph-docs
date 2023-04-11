---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReview()
request_body.displayName = 'TestReview new name'



request_configuration = AccessReviewRequestBuilderPatchRequestConfiguration(
)


result = await client.accessReviews_by_id('accessReview-id').patch(request_body = request_body)


```