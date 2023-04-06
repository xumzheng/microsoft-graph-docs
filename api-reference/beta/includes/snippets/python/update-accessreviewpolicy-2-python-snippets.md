---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewPolicy()
request_body.setIsGroupOwnerManagementEnabled(true)


request_config = PolicyRequestBuilderPatchRequestConfiguration(
request_config = PolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityGovernance.accessReviews.policy.patch(request_body, headers=)


```