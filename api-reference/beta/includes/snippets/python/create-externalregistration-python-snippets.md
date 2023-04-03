---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RegistrationPostRequestBody();
additionalData = [
'@odata.type' => '#microsoft.graph.externalMeetingRegistration', 
'allowedRegistrant' => 'everyone', 
];
requestBody.setAdditionalData(additionalData);




await client.me().onlineMeetingsById('onlineMeeting-id').registration().post(requestBody);


```