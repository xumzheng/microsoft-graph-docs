---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Decision();
additionalData = [
'decision' => 'Approve', 
'justification' => 'The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources', 
];
requestBody.setAdditionalData(additionalData);




await client.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').decisionsById('accessReviewInstanceDecisionItem-id').post(requestBody);


```