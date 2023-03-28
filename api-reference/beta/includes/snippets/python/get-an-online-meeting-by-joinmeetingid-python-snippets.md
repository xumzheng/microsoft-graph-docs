---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new OnlineMeetingsRequestBuilderGetRequestConfiguration();

$queryParameters = new OnlineMeetingsRequestBuilderGetQueryParameters();
$queryParameters->filter = "joinMeetingIdSettings/joinMeetingId eq '1234567890'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->me()->onlineMeetings()->get($requestConfiguration);


```