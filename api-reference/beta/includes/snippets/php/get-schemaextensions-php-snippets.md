---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SchemaExtensionsRequestBuilderGetRequestConfiguration();

$queryParameters = new SchemaExtensionsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'id%20eq%20\'graphlearn_test\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->schemaExtensions()->get($requestConfiguration);


```