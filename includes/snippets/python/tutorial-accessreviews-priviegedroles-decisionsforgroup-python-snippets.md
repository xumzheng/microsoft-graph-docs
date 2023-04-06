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



request_config = AccessReviewInstanceDecisionItemRequestBuilderPostRequestConfiguration(
request_config = AccessReviewInstanceDecisionItemRequestBuilderPostRequestConfiguration(query_params=)


await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances_by_id('accessReviewInstance-id').decisions_by_id('accessReviewInstanceDecisionItem-id').post(request_body, headers=)


```