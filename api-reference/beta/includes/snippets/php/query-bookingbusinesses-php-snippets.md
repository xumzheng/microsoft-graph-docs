---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new BookingBusinessesRequestBuilderGetRequestConfiguration();

$queryParameters = new BookingBusinessesRequestBuilderGetQueryParameters();
$queryParameters->query = 'Adventure';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->bookingBusinesses()->get($requestConfiguration);


```