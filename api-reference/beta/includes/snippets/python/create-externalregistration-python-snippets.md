---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RegistrationPostRequestBody()
additionalData = [
'@odata.type' => '#microsoft.graph.externalMeetingRegistration', 
'allowedRegistrant' => 'everyone', 
];
request_body.setAdditionalData(additionalData)




await client.me.onlineMeetings_by_id('onlineMeeting-id').registration.post(request_body)


```