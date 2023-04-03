---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RecordResponsePostRequestBody();
requestBody.setBargeInAllowed(true);

requestBody.setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');

promptsPrompt1 = Prompt();
promptsPrompt1.set@odatatype('#microsoft.graph.mediaPrompt');

additionalData = [
'mediaInfo' => promptsPrompt1 = MediaInfo();
		promptsPrompt1.setUri('https://cdn.contoso.com/beep.wav');

		promptsPrompt1.setResourceId('1D6DE2D4-CD51-4309-8DAA-70768651088E');


promptsPrompt1.setMediaInfo($mediaInfo);

];
promptsPrompt1.setAdditionalData(additionalData);



promptsArray []= promptsPrompt1;
requestBody.setPrompts(promptsArray);


requestBody.setMaxRecordDurationInSeconds(10);

requestBody.setInitialSilenceTimeoutInSeconds(5);

requestBody.setMaxSilenceTimeoutInSeconds(2);

requestBody.setPlayBeep(true);

requestBody.setStopTones(['#', '1', '*', ]);



result = awaitclient.communications().callsById('call-id').recordResponse().post(requestBody);


```