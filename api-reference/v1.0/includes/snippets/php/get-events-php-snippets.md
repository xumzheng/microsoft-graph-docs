---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new EventsRequestBuilderGetRequestConfiguration();

$queryParameters = new EventsRequestBuilderGetQueryParameters();
$queryParameters->select = 'subject,body,bodyPreview,organizer,attendees,start,end,location';

$headers = [
"Prefer" => "outlook.timezone=\"Pacific Standard Time\"",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->me()->events()->get($requestConfiguration);


```