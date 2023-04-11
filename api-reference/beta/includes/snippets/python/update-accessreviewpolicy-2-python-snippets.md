---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewPolicy()
request_body.isGroupOwnerManagementEnabled = true



request_configuration = PolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.identityGovernance.accessReviews.policy.patch(request_body = request_body)


```