---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AnswerPostRequestBody()
request_body.callbackUri = 'callbackUri-value'

media_config = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.appHostedMediaConfig'

additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
mediaConfig.additionaldata(additionalData)



request_body.media_config = mediaConfig
request_body.AcceptedModalities([request_body.Modality(Modality('audio'))
])

call_options = IncomingCallOptions()
callOptions.@odatatype = '#microsoft.graph.incomingCallOptions'

callOptions.is_content_sharing_notification_enabled = True


request_body.call_options = callOptions
request_body.participant_capacity = 200




await client.communications.calls_by_id('call-id').answer.post(request_body = request_body)


```