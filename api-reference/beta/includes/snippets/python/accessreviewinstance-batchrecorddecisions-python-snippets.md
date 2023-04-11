---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BatchRecordDecisionsPostRequestBody()
request_body.decision = 'Approve'

request_body.justification = 'All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team'

request_body.resourceId = 'a5c51e59-3fcd-4a37-87a1-835c0c21488a'



request_configuration = BatchRecordDecisionsRequestBuilderPostRequestConfiguration(
)


await client.me.pendingAccessReviewInstances_by_id('accessReviewInstance-id').batchRecordDecisions.post(request_body = request_body)


```