---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RegistrationRequestBuilderGetRequestConfiguration();

$queryParameters = new RegistrationRequestBuilderGetQueryParameters();
$queryParameters->expand = 'microsoft.graph.meetingRegistration/customQuestions';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->get($requestConfiguration);


```