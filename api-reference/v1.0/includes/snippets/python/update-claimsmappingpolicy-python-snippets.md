---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ClaimsMappingPolicy()
request_body.setDisplayName('UpdateClaimsPolicy')



result = await client.policies.claimsMappingPoliciesby_id('claimsMappingPolicy-id').patch(request_body)


```