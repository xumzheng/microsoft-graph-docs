---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReviewPolicy()
request_body.setIsGroupOwnerManagementEnabled(true)


request_config = AccessReviewPolicyRequestBuilderPatchRequestConfiguration(
request_config = AccessReviewPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.accessReviewPolicy.patch(request_body, headers=)


```