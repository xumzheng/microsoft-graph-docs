---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new InstancesRequestBuilderGetRequestConfiguration();

$queryParameters = new InstancesRequestBuilderGetQueryParameters();
$queryParameters->startDateTime = '2019-04-08T09:00:00.0000000';
$queryParameters->endDateTime = '2019-04-30T09:00:00.0000000';
$queryParameters->select = 'subject,bodyPreview,seriesMasterId,type,recurrence,start,end';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->eventsById('event-id')->instances()->get($requestConfiguration);


```