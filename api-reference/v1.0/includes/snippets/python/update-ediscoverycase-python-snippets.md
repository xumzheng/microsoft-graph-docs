---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCase()
request_body.setDisplayName('My Case 1 - Renamed')

request_body.setDescription('Updated description')


request_config = EdiscoveryCaseRequestBuilderPatchRequestConfiguration(
request_config = EdiscoveryCaseRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').patch(request_body, headers=)


```