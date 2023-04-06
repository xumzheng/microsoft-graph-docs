---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration(
request_configuration = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration(query_params=query_params = EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters()
query_params['expand'] = ["dataSource"]

)
query_params = EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters()
query_params['expand'] = ["dataSource"]

)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources_by_id('ediscoveryNoncustodialDataSource-id').get(request_configuration)


```