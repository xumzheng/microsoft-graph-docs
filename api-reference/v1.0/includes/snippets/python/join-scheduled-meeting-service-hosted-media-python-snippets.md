---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.callbackUri = 'https://bot.contoso.com/callback'

request_body.RequestedModalities([request_body.Modality(Modality('audio'))
])

media_config = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.serviceHostedMediaConfig'

additionalData = [
'preFetchMedia' => pre_fetch_media1 = ()
	preFetchMedia1.uri = 'https://cdn.contoso.com/beep.wav'

	preFetchMedia1.resourceId = 'f8971b04-b53e-418c-9222-c82ce681a582'


preFetchMediaArray []= preFetchMedia1;
pre_fetch_media2 = ()
	preFetchMedia2.uri = 'https://cdn.contoso.com/cool.wav'

	preFetchMedia2.resourceId = '86dc814b-c172-4428-9112-60f8ecae1edb'


preFetchMediaArray []= preFetchMedia2;
mediaConfig.prefetchmedia(preFetchMediaArray)


];
mediaConfig.additionaldata(additionalData)



request_body.media_config = mediaConfig
chat_info = ChatInfo()
chatInfo.@odatatype = '#microsoft.graph.chatInfo'

chatInfo.threadId = '19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2'

chatInfo.messageId = '0'


request_body.chat_info = chatInfo
meeting_info = MeetingInfo()
meetingInfo.@odatatype = '#microsoft.graph.organizerMeetingInfo'

additionalData = [
'organizer' => meeting_info = Organizer()
meetingInfo.@odatatype = '#microsoft.graph.identitySet'

user = User()
user.@odatatype = '#microsoft.graph.identity'

user.id = '5810cede-f3cc-42eb-b2c1-e9bd5d53ec96'

user.displayName = 'Bob'

user.tenantId = '86dc81db-c112-4228-9222-63f3esaa1edb'


meetingInfo.user = user

meetingInfo.organizer = organizer

'allowConversationWithoutHost' => true,
];
meetingInfo.additionaldata(additionalData)



request_body.meeting_info = meetingInfo
request_body.tenantId = '86dc81db-c112-4228-9222-63f3esaa1edb'




result = await client.communications.calls.post(request_body = request_body)


```