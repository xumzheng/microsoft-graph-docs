---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = FilesRequestBuilderGetRequestConfiguration(
request_configuration = FilesRequestBuilderGetRequestConfiguration(query_params=query_params = FilesRequestBuilderGetQueryParameters()
query_params['top'] = 5

)
query_params = FilesRequestBuilderGetQueryParameters()
query_params['top'] = 5

)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').reviewSets_by_id('ediscoveryReviewSet-id').files.get(request_configuration)


```