---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MuteAllPostRequestBody();
$requestBody.setParticipants(['', ]);

$requestBody.setClientContext('clientContext-value');



$requestResult = $graphServiceClient.communications().callsById('call-id').participants().muteAll().post($requestBody);


```