---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LegalHold()
request_body.setDescription('This is a description for a legalHold')


request_config = LegalHoldRequestBuilderPatchRequestConfiguration(
request_config = LegalHoldRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.compliance.ediscovery.cases_by_id('case-id').legalHolds_by_id('legalHold-id').patch(request_body, headers=)


```