---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new NamedLocationsRequestBuilderGetRequestConfiguration();

$queryParameters = new NamedLocationsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'createdDateTime%20ge%202019-09-01T00:00:00Z';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->conditionalAccess()->namedLocations()->get($requestConfiguration);


```