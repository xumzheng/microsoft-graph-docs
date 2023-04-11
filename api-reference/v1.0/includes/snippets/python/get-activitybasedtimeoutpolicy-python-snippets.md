---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = ActivityBasedTimeoutPolicyRequestBuilderGetRequestConfiguration(
)


result = await client.policies.activityBasedTimeoutPolicies_by_id('activityBasedTimeoutPolicy-id').get()


```