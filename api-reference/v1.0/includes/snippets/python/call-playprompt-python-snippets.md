---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlayPromptPostRequestBody()
request_body.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c')

promptsPrompt1 = Prompt()
promptsPrompt1.set@odatatype('#microsoft.graph.mediaPrompt')

additionalData = [
'mediaInfo' => promptsPrompt1 = MediaInfo()
		promptsPrompt1.set@odatatype('#microsoft.graph.mediaInfo')

		promptsPrompt1.setUri('https://cdn.contoso.com/beep.wav')

		promptsPrompt1.setResourceId('1D6DE2D4-CD51-4309-8DAA-70768651088E')


promptsPrompt1.setMediaInfo($mediaInfo)

];
promptsPrompt1.setAdditionalData(additionalData)



promptsArray []= promptsPrompt1;
request_body.setPrompts(promptsArray)




result = await client.communications.calls._by_id('call-id').playPrompt.post(request_body)


```