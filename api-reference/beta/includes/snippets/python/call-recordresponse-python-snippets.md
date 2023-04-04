---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RecordResponsePostRequestBody()
request_body.setBargeInAllowed(true)

request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')

promptsPrompt1 = Prompt()
promptsPrompt1.set@odatatype('#microsoft.graph.mediaPrompt')

additionalData = [
'mediaInfo' => promptsPrompt1 = MediaInfo()
		promptsPrompt1.setUri('https://cdn.contoso.com/beep.wav')

		promptsPrompt1.setResourceId('1D6DE2D4-CD51-4309-8DAA-70768651088E')


promptsPrompt1.setMediaInfo($mediaInfo)

];
promptsPrompt1.setAdditionalData(additionalData)



promptsArray []= promptsPrompt1;
request_body.setPrompts(promptsArray)


request_body.setMaxRecordDurationInSeconds(10)

request_body.setInitialSilenceTimeoutInSeconds(5)

request_body.setMaxSilenceTimeoutInSeconds(2)

request_body.setPlayBeep(true)

request_body.setStopTones(['#', '1', '*', ])



result = await client.communications.callsById('call-id').recordResponse.post(request_body)


```