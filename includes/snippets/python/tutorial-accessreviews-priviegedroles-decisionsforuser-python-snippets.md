---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Decision();
additionalData = [
'decision' => 'Deny', 
'justification' => 'Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy \'#132487: Privileged roles\'', 
];
requestBody.setAdditionalData(additionalData);




await client.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').decisionsById('accessReviewInstanceDecisionItem-id').post(requestBody);


```