---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new FilesRequestBuilderGetRequestConfiguration();

$queryParameters = new FilesRequestBuilderGetQueryParameters();
$queryParameters->top = 5;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->reviewSetsById('ediscoveryReviewSet-id')->files()->get($requestConfiguration);


```