---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = NoncustodialDataSourcesRequestBuilderGetRequestConfiguration(
request_config = NoncustodialDataSourcesRequestBuilderGetRequestConfiguration(query_params=query_params = NoncustodialDataSourcesRequestBuilderGetQueryParameters()
query_params.expand = ["dataSource"]

)
query_params = NoncustodialDataSourcesRequestBuilderGetQueryParameters()
query_params.expand = ["dataSource"]

)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources.get(request_config, headers=request_config)


```