---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewInstanceDecisionItem()
request_body.decision = 'Approve'

request_body.justification = 'This person is still on my team'



request_configuration = AccessReviewInstanceDecisionItemRequestBuilderPatchRequestConfiguration(
)


result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances_by_id('accessReviewInstance-id').stages_by_id('accessReviewStage-id').decisions_by_id('accessReviewInstanceDecisionItem-id').patch(request_body = request_body)


```