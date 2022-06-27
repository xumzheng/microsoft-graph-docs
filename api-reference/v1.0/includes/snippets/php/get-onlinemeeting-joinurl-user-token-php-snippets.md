---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OnlineMeetingsRequestBuilderGetRequestConfiguration();

$queryParameters = new OnlineMeetingsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'JoinWebUrl%20eq%20\'https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->onlineMeetings()->get($requestConfiguration);


```