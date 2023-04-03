---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AccessReviewInstanceDecisionItem();
requestBody.setDecision('Approve');

requestBody.setJustification('This person is still on my team');



result = await client.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').stagesById('accessReviewStage-id').decisionsById('accessReviewInstanceDecisionItem-id').patch(requestBody);


```