---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = BatchRecordDecisionsPostRequestBody();
request_body.setDecision('Approve');

request_body.setJustification('All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team');

request_body.setResourceId('a5c51e59-3fcd-4a37-87a1-835c0c21488a');



await client.identityGovernance.accessReviews.definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').batchRecordDecisions.post(request_body);


```