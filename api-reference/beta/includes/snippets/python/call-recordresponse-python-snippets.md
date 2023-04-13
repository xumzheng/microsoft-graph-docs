---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RecordResponsePostRequestBody()
request_body.barge_in_allowed = True

request_body.clientContext = 'd45324c1-fcb5-430a-902c-f20af696537c'

prompts_prompt1 = Prompt()
promptsPrompt1.@odatatype = '#microsoft.graph.mediaPrompt'

additionalData = [
'mediaInfo' => prompts_prompt1 = MediaInfo()
		promptsPrompt1.uri = 'https://cdn.contoso.com/beep.wav'

		promptsPrompt1.resourceId = '1D6DE2D4-CD51-4309-8DAA-70768651088E'


promptsPrompt1.media_info = mediaInfo

];
promptsPrompt1.additionaldata(additionalData)



promptsArray []= promptsPrompt1;
request_body.prompts(promptsArray)


request_body.max_record_duration_in_seconds = 10

request_body.initial_silence_timeout_in_seconds = 5

request_body.max_silence_timeout_in_seconds = 2

request_body.play_beep = True

request_body.StopTones(['#', '1', '*', ])




result = await client.communications.calls_by_id('call-id').recordResponse.post(request_body = request_body)


```