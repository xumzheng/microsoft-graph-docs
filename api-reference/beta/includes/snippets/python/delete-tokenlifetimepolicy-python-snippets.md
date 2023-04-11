---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = TokenLifetimePolicyRequestBuilderDeleteRequestConfiguration(
)


await client.policies.tokenLifetimePolicies_by_id('tokenLifetimePolicy-id').delete()


```