---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AnswerPostRequestBody();
requestBody.setCallbackUri('callbackUri-value');

mediaConfig = MediaConfig();
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig');

additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
mediaConfig.setAdditionalData(additionalData);



requestBody.setMediaConfig($mediaConfig);
requestBody.setAcceptedModalities([requestBody.setModality(Modality('audio'));
]);

callOptions = IncomingCallOptions();
callOptions.set@odatatype('#microsoft.graph.incomingCallOptions');

callOptions.setIsContentSharingNotificationEnabled(true);


requestBody.setCallOptions($callOptions);
requestBody.setParticipantCapacity(200);



awaitclient.communications().callsById('call-id').answer().post(requestBody);


```