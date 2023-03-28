---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CalendarViewRequestBuilderGetRequestConfiguration();

$queryParameters = new CalendarViewRequestBuilderGetQueryParameters();
$queryParameters.start = "2018-04-30T00:00:00Z";
$queryParameters.end = "2018-05-10T00:00:00Z";

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.solutions().bookingBusinessesById('bookingBusiness-id').calendarView().get($requestConfiguration);


```