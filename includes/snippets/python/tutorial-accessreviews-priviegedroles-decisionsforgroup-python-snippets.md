---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Decision()
additionalData = [
'decision' => 'Approve', 
'justification' => 'The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources', 
];
request_body.setAdditionalData(additionalData)




await client.identityGovernance.accessReviews.definitions._by_id('accessReviewScheduleDefinition-id').instances._by_id('accessReviewInstance-id').decisions._by_id('accessReviewInstanceDecisionItem-id').post(request_body)


```