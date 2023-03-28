---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new RegistrationRequestBuilderGetRequestConfiguration();

$queryParameters = new RegistrationRequestBuilderGetQueryParameters();
$queryParameters->expand = ["microsoft.graph.meetingRegistration/customQuestions"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->get($requestConfiguration);


```