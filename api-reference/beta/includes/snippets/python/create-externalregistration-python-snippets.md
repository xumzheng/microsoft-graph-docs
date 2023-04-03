---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RegistrationPostRequestBody();
additionalData = [
'@odata.type' => '#microsoft.graph.externalMeetingRegistration', 
'allowedRegistrant' => 'everyone', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.me().onlineMeetingsById('onlineMeeting-id').registration().post(requestBody);


```