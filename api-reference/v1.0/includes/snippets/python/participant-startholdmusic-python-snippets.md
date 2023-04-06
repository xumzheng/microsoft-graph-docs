---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = StartHoldMusicPostRequestBody()
customPrompt = Prompt()
customPrompt.set@odatatype('#microsoft.graph.mediaPrompt')

additionalData = [
'mediaInfo' => customPrompt = MediaInfo()
		customPrompt.set@odatatype('#microsoft.graph.mediaInfo')

		customPrompt.setUri('https://bot.contoso.com/onHold.wav')


customPrompt.setMediaInfo($mediaInfo)

];
customPrompt.setAdditionalData(additionalData)



request_body.setCustomPrompt($customPrompt)
request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')



result = await client.communications.calls_by_id('call-id').participants_by_id('participant-id').startHoldMusic.post(request_body, headers=)


```