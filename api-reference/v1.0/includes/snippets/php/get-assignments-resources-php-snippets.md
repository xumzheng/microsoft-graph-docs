---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AssignmentsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'resources';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->education()->classesById('educationClass-id')->assignments()->get($requestConfiguration);


```