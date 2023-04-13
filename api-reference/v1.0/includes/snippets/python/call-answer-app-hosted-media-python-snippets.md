---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AnswerPostRequestBody()
request_body.callbackUri = 'https://bot.contoso.com/api/calls'

request_body.AcceptedModalities([request_body.Modality(Modality('audio'))
])

media_config = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.appHostedMediaConfig'

additionalData = [
'blob' => '<Media Session Configuration Blob>', 
];
mediaConfig.additionaldata(additionalData)



request_body.media_config = mediaConfig



await client.communications.calls_by_id('call-id').answer.post(request_body = request_body)


```