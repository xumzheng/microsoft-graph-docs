---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ContentRequestBuilderGetRequestConfiguration();

$queryParameters = new ContentRequestBuilderGetQueryParameters();
$queryParameters.format = "text/vtt";

$headers = [
'Accept' => 'application/vnd.openxmlformats-officedocument.wordprocessingml.document',
];

$requestConfiguration.queryParameters = $queryParameters;
$requestConfiguration.headers = $headers;


$graphServiceClient.usersById('user-id').onlineMeetingsById('onlineMeeting-id').transcriptsById('callTranscript-id').content().get($requestConfiguration);


```