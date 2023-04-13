---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewStage()
request_body.@odatatype = '#microsoft.graph.accessReviewStage'

reviewers_access_review_reviewer_scope1 = AccessReviewReviewerScope()
reviewersAccessReviewReviewerScope1.query = '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5'

reviewersAccessReviewReviewerScope1.queryType = 'MicrosoftGraph'


reviewersArray []= reviewersAccessReviewReviewerScope1;
request_body.reviewers(reviewersArray)


fallback_reviewers_access_review_reviewer_scope1 = AccessReviewReviewerScope()
fallbackReviewersAccessReviewReviewerScope1.query = '/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e'

fallbackReviewersAccessReviewReviewerScope1.queryType = 'MicrosoftGraph'


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope1;
fallback_reviewers_access_review_reviewer_scope2 = AccessReviewReviewerScope()
fallbackReviewersAccessReviewReviewerScope2.query = '/users/1ed8ac56-4827-4733-8f80-86adc2e67db5'

fallbackReviewersAccessReviewReviewerScope2.queryType = 'MicrosoftGraph'


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope2;
request_body.fallbackreviewers(fallbackReviewersArray)





result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances_by_id('accessReviewInstance-id').stages_by_id('accessReviewStage-id').patch(request_body = request_body)


```