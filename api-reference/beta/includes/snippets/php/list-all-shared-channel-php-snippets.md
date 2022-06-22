---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AllChannelsRequestBuilderGetRequestConfiguration();

$queryParameters = new AllChannelsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'membershipType%20eq%20\'shared\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->allChannels()->get($requestConfiguration);


```