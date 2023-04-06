---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SourceCollection()
request_body.setDisplayName('Quarterly Financials search')


request_config = SourceCollectionRequestBuilderPatchRequestConfiguration(
request_config = SourceCollectionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').patch(request_body, headers=)


```