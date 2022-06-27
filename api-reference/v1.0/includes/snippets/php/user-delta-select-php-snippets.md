---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->select = 'displayName,jobTitle,mobilePhone';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->users()->delta()()->get($requestConfiguration);


```