---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ProfileRequestBuilderGetRequestConfiguration();

$queryParameters = new ProfileRequestBuilderGetQueryParameters();
$queryParameters->expand = 'names($select=first,last),skills($select=displayName)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->profile()->get($requestConfiguration);


```