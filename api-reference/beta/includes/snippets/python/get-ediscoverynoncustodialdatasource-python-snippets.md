---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = EdiscoveryNoncustodialDataSourceRequestBuilder.EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters(
				expand = ["dataSource"],
)

request_configuration = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources_by_id('ediscoveryNoncustodialDataSource-id').get(request_configuration = request_configuration)


```