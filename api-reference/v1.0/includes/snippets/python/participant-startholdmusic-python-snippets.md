---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = StartHoldMusicPostRequestBody()
custom_prompt = Prompt()
customPrompt.@odatatype = '#microsoft.graph.mediaPrompt'

additionalData = [
'mediaInfo' => custom_prompt = MediaInfo()
		customPrompt.@odatatype = '#microsoft.graph.mediaInfo'

		customPrompt.uri = 'https://bot.contoso.com/onHold.wav'


customPrompt.media_info = mediaInfo

];
customPrompt.additionaldata(additionalData)



request_body.custom_prompt = customPrompt
request_body.clientContext = 'd45324c1-fcb5-430a-902c-f20af696537c'




result = await client.communications.calls_by_id('call-id').participants_by_id('participant-id').startHoldMusic.post(request_body = request_body)


```