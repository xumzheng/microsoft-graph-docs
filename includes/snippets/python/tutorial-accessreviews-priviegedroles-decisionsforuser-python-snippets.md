---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Decision();
additionalData = [
'decision' => 'Deny', 
'justification' => 'Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy \'#132487: Privileged roles\'', 
];
request_body.setAdditionalData(additionalData);




await client.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').decisionsById('accessReviewInstanceDecisionItem-id').post(request_body);


```