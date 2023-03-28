---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new NoncustodialDataSourcesRequestBuilderGetRequestConfiguration();

$queryParameters = new NoncustodialDataSourcesRequestBuilderGetQueryParameters();
$queryParameters->expand = ["dataSource"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->noncustodialDataSources()->get($requestConfiguration);


```