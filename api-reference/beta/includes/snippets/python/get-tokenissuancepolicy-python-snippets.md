---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = TokenIssuancePolicyRequestBuilderGetRequestConfiguration(
)


result = await client.policies.tokenIssuancePolicies_by_id('tokenIssuancePolicy-id').get()


```