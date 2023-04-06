---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.set@odatatype('#microsoft.graph.call')

request_body.setCallbackUri('https://bot.contoso.com/callback')

request_body.setRequestedModalities([request_body.setModality(Modality('audio'))
])

mediaConfig = MediaConfig()
mediaConfig.set@odatatype('#microsoft.graph.serviceHostedMediaConfig')

additionalData = [
'preFetchMedia' => preFetchMedia1 = ()
	preFetchMedia1.setUri('https://cdn.contoso.com/beep.wav')

	preFetchMedia1.setResourceId('f8971b04-b53e-418c-9222-c82ce681a582')


preFetchMediaArray []= preFetchMedia1;
preFetchMedia2 = ()
	preFetchMedia2.setUri('https://cdn.contoso.com/cool.wav')

	preFetchMedia2.setResourceId('86dc814b-c172-4428-9112-60f8ecae1edb')


preFetchMediaArray []= preFetchMedia2;
mediaConfig.setPreFetchMedia(preFetchMediaArray)


];
mediaConfig.setAdditionalData(additionalData)



request_body.setMediaConfig($mediaConfig)
meetingInfo = MeetingInfo()
meetingInfo.set@odatatype('#microsoft.graph.joinMeetingIdMeetingInfo')

additionalData = [
'joinMeetingId' => '1234567', 
'passcode' => null,
];
meetingInfo.setAdditionalData(additionalData)



request_body.setMeetingInfo($meetingInfo)
request_body.setTenantId('86dc81db-c112-4228-9222-63f3esaa1edb')



result = await client.communications.calls.post(request_body, headers=)


```