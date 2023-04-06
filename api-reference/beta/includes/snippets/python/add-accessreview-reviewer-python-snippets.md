---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewReviewer()
request_body.setId('006111db-0810-4494-a6df-904d368bd81b')


request_config = ReviewersRequestBuilderPostRequestConfiguration(
request_config = ReviewersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.accessReviews_by_id('accessReview-id').reviewers.post(request_body, headers=)


```