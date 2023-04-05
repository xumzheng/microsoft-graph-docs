---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReview()
request_body.setDisplayName('TestReview new name')



result = await client.accessReviewsById('accessReview-id').patch(request_body)


```