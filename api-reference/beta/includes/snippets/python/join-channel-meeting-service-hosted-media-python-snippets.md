---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

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
chatInfo = ChatInfo()
chatInfo.set@odatatype('#microsoft.graph.chatInfo')

chatInfo.setThreadId('19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype')

chatInfo.setMessageId('1533758867081')


request_body.setChatInfo($chatInfo)
meetingInfo = MeetingInfo()
meetingInfo.set@odatatype('#microsoft.graph.organizerMeetingInfo')

meetingInfo.setAllowConversationWithoutHost(true)

additionalData = [
'organizer' => meetingInfo = Organizer()
meetingInfo.set@odatatype('#microsoft.graph.identitySet')

user = User()
user.set@odatatype('#microsoft.graph.identity')

user.setId('5810cede-f3cc-42eb-b2c1-e9bd5d53ec96')

user.setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a')

user.setDisplayName('Bob')


meetingInfo.setUser($user)

meetingInfo.setOrganizer($organizer)

];
meetingInfo.setAdditionalData(additionalData)



request_body.setMeetingInfo($meetingInfo)


result = await client.communications.calls.post(request_body)


```