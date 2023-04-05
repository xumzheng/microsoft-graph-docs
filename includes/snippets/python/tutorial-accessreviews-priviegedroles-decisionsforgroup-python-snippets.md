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




await client.identityGovernance_accessReviews_definitionsby_id('accessReviewScheduleDefinition-id')_instancesby_id('accessReviewInstance-id')_decisionsby_id('accessReviewInstanceDecisionItem-id').post(request_body)


```