---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessReviewInstanceDecisionItem();
$requestBody.setDecision('Approve');

$requestBody.setJustification('This person is still on my team');



$requestResult = $graphServiceClient.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').stagesById('accessReviewStage-id').decisionsById('accessReviewInstanceDecisionItem-id').patch($requestBody);


```