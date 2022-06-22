---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new EdiscoveryNoncustodialDataSourceRequestBuilderGetRequestConfiguration();

$queryParameters = new EdiscoveryNoncustodialDataSourceRequestBuilderGetQueryParameters();
$queryParameters->expand = 'dataSource';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->noncustodialDataSourcesById('ediscoveryNoncustodialDataSource-id')->get($requestConfiguration);


```