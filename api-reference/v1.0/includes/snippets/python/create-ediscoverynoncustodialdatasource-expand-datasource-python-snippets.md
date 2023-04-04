---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = NoncustodialDataSourcesRequestBuilderGetRequestConfiguration();

query_params = NoncustodialDataSourcesRequestBuilderGetQueryParameters();
query_params.expand = ["dataSource"];

request_config.queryParameters = query_params;


result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').noncustodialDataSources.get(request_config);


```