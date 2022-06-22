---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new EventRequestBuilderGetRequestConfiguration();

$queryParameters = new EventRequestBuilderGetQueryParameters();
$queryParameters->select = 'subject,body,bodyPreview,organizer,attendees,start,end,location,locations';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->eventsById('event-id')->get($requestConfiguration);


```