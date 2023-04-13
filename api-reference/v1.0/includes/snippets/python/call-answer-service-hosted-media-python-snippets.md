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
mediaConfig.@odatatype = '#microsoft.graph.serviceHostedMediaConfig'

additionalData = [
'preFetchMedia' => pre_fetch_media1 = ()
	preFetchMedia1.uri = 'https://cdn.contoso.com/beep.wav'

	preFetchMedia1.resourceId = '1D6DE2D4-CD51-4309-8DAA-70768651088E'


preFetchMediaArray []= preFetchMedia1;
pre_fetch_media2 = ()
	preFetchMedia2.uri = 'https://cdn.contoso.com/cool.wav'

	preFetchMedia2.resourceId = '1D6DE2D4-CD51-4309-8DAA-70768651088F'


preFetchMediaArray []= preFetchMedia2;
mediaConfig.prefetchmedia(preFetchMediaArray)


];
mediaConfig.additionaldata(additionalData)



request_body.media_config = mediaConfig



await client.communications.calls_by_id('call-id').answer.post(request_body = request_body)


```