---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GetAllMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new GetAllMessagesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'lastModifiedDateTime%20gt%202019-11-01T00:00:00Z%20and%20lastModifiedDateTime%20lt%202021-11-01T00:00:00Z';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->channels()->getAllMessages()()->get($requestConfiguration);


```