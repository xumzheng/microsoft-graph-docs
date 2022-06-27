---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TimesOffRequestBuilderGetRequestConfiguration();

$queryParameters = new TimesOffRequestBuilderGetQueryParameters();
$queryParameters->filter = 'sharedTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20sharedTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z%20and%20draftTimeOff/startDateTime%20ge%202019-03-11T00:00:00.000Z%20and%20draftTimeOff/endDateTime%20le%202019-03-18T00:00:00.000Z';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->schedule()->timesOff()->get($requestConfiguration);


```