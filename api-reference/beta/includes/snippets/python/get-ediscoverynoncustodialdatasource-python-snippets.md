---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration(
request_config = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration(query_params=query_params = EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters()
query_params.expand = ["dataSource"]

)
query_params = EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters()
query_params.expand = ["dataSource"]

)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources_by_id('ediscoveryNoncustodialDataSource-id').get(request_config, headers=request_config)


```