---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryHoldPolicy()
request_body.setDescription('updated description')


request_config = EdiscoveryHoldPolicyRequestBuilderPatchRequestConfiguration(
request_config = EdiscoveryHoldPolicyRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').legalHolds_by_id('ediscoveryHoldPolicy-id').patch(request_body, headers=)


```