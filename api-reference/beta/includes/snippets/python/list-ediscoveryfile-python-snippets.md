---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = FilesRequestBuilderGetRequestConfiguration()

query_params = FilesRequestBuilderGetQueryParameters()
query_params.top = 5

request_config.queryParameters = query_params


result = await client.security.cases.ediscoveryCasesby_id('ediscoveryCase-id').reviewSetsby_id('ediscoveryReviewSet-id').files.get(request_config)


```