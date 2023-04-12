---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RecordResponsePostRequestBody()
request_body.bargeInAllowed = true

request_body.clientContext = 'd45324c1-fcb5-430a-902c-f20af696537c'

promptsPrompt1 = Prompt()
promptsPrompt1.@odatatype = '#microsoft.graph.mediaPrompt'

additionalData = [
'mediaInfo' => promptsPrompt1 = MediaInfo()
		promptsPrompt1.uri = 'https://cdn.contoso.com/beep.wav'

		promptsPrompt1.resourceId = '1D6DE2D4-CD51-4309-8DAA-70768651088E'


promptsPrompt1.mediaInfo = mediaInfo

];
promptsPrompt1.additionaldata(additionalData)



promptsArray []= promptsPrompt1;
request_body.prompts(promptsArray)


request_body.maxRecordDurationInSeconds = 10

request_body.initialSilenceTimeoutInSeconds = 5

request_body.maxSilenceTimeoutInSeconds = 2

request_body.playBeep = true

request_body.StopTones(['#', '1', '*', ])




result = await client.communications.calls_by_id('call-id').recordResponse.post(request_body = request_body)


```