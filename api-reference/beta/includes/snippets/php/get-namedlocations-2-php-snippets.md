---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new NamedLocationsRequestBuilderGetRequestConfiguration();

$queryParameters = new NamedLocationsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'isof(\'microsoft.graph.ipNamedLocation\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->conditionalAccess()->namedLocations()->get($requestConfiguration);


```