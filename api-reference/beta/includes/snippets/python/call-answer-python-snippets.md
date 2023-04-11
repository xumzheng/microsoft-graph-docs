---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AnswerPostRequestBody()
request_body.callbackUri = 'callbackUri-value'

mediaConfig = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.appHostedMediaConfig'

additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
mediaConfig.additionaldata(additionalData)



request_body.mediaConfig = mediaConfig
request_body.AcceptedModalities([request_body.Modality(Modality('audio'))
])

callOptions = IncomingCallOptions()
callOptions.@odatatype = '#microsoft.graph.incomingCallOptions'

callOptions.isContentSharingNotificationEnabled = true


request_body.callOptions = callOptions
request_body.participantCapacity = 200



request_configuration = AnswerRequestBuilderPostRequestConfiguration(
)


await client.communications.calls_by_id('call-id').answer.post(request_body = request_body)


```