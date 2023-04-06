---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AnswerPostRequestBody()
request_body.setCallbackUri('callbackUri-value')

mediaConfig = MediaConfig()
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig')

additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
mediaConfig.setAdditionalData(additionalData)



request_body.setMediaConfig($mediaConfig)
request_body.setAcceptedModalities([request_body.setModality(Modality('audio'))
])

callOptions = IncomingCallOptions()
callOptions.set@odatatype('#microsoft.graph.incomingCallOptions')

callOptions.setIsContentSharingNotificationEnabled(true)


request_body.setCallOptions($callOptions)
request_body.setParticipantCapacity(200)


request_config = AnswerRequestBuilderPostRequestConfiguration(
request_config = AnswerRequestBuilderPostRequestConfiguration(query_params=)


await client.communications.calls_by_id('call-id').answer.post(request_body, headers=)


```