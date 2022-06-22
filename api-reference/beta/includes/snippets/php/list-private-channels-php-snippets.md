---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ChannelsRequestBuilderGetRequestConfiguration();

$queryParameters = new ChannelsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'membershipType%20eq%20\'private\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->channels()->get($requestConfiguration);


```