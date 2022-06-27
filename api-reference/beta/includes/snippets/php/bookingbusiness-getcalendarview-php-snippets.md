---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CalendarViewRequestBuilderGetRequestConfiguration();

$queryParameters = new CalendarViewRequestBuilderGetQueryParameters();
$queryParameters->start = '2018-04-30T00:00:00Z';
$queryParameters->end = '2018-05-10T00:00:00Z';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->calendarView()->get($requestConfiguration);


```