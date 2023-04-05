---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewInstanceDecisionItem()
request_body.setDecision('Approve')

request_body.setJustification('This person is still on my team')



result = await client.identityGovernance.accessReviews.definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').stagesById('accessReviewStage-id').decisionsById('accessReviewInstanceDecisionItem-id').patch(request_body)


```