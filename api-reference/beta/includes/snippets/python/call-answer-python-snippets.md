---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AnswerPostRequestBody();
$requestBody.setCallbackUri('callbackUri-value');

$mediaConfig = new MediaConfig();
$mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig');

$additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
$mediaConfig.setAdditionalData($additionalData);



$requestBody.setMediaConfig($mediaConfig);
$requestBody.setAcceptedModalities([$requestBody.setModality(new Modality('audio'));
]);

$callOptions = new IncomingCallOptions();
$callOptions.set@odatatype('#microsoft.graph.incomingCallOptions');

$callOptions.setIsContentSharingNotificationEnabled(true);


$requestBody.setCallOptions($callOptions);
$requestBody.setParticipantCapacity(200);



$graphServiceClient.communications().callsById('call-id').answer().post($requestBody);


```