---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = NoncustodialDataSourcesRequestBuilderGetRequestConfiguration();

queryParameters = NoncustodialDataSourcesRequestBuilderGetQueryParameters();
queryParameters.expand = ["dataSource"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').noncustodialDataSources().get(requestConfiguration);


```