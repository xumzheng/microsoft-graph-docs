---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CalendarViewRequestBuilderGetRequestConfiguration();

$queryParameters = new CalendarViewRequestBuilderGetQueryParameters();
$queryParameters->startDateTime = '2017-01-01T19:00:00-08:00';
$queryParameters->endDateTime = '2017-10-01T19:00:00.00-08:00';

$headers = [
"Prefer" => "outlook.body-content-type=\"text\"",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->groupsById('group-id')->calendarView()->get($requestConfiguration);


```