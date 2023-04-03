---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = BatchRecordDecisionsPostRequestBody();
requestBody.setDecision('Approve');

requestBody.setJustification('All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team');

requestBody.setResourceId('a5c51e59-3fcd-4a37-87a1-835c0c21488a');



await client.me().pendingAccessReviewInstancesById('accessReviewInstance-id').batchRecordDecisions().post(requestBody);


```