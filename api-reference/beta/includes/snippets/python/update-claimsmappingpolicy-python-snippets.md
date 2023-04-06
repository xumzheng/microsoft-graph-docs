---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClaimsMappingPolicy()
request_body.setDisplayName('UpdateClaimsPolicy')


request_config = ClaimsMappingPolicyRequestBuilderPatchRequestConfiguration(
request_config = ClaimsMappingPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.policies.claimsMappingPolicies_by_id('claimsMappingPolicy-id').patch(request_body, headers=)


```