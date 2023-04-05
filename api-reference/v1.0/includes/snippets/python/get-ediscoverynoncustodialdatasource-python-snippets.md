---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration()

query_params = EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters()
query_params.expand = ["dataSource"]

request_config.queryParameters = query_params


result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_noncustodialDataSourcesby_id('ediscoveryNoncustodialDataSource-id').get(request_config)


```