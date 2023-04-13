---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.callbackUri = 'https://bot.contoso.com/callback'

source = ParticipantInfo()
source.@odatatype = '#microsoft.graph.participantInfo'

source_identity = IdentitySet()
sourceIdentity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'guest' => source_identity = Guest()
		sourceIdentity.@odatatype = '#microsoft.graph.identity'

		sourceIdentity.displayName = 'Guest User'

		sourceIdentity.id = 'd7a3b999-17ac-4bca-9e77-e6a730d2ec2e'


sourceIdentity.guest = guest

];
sourceIdentity.additionaldata(additionalData)



source.identity = sourceIdentity

request_body.source = source
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

chatInfo.threadId = '19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype'

chatInfo.messageId = '1533758867081'


request_body.chat_info = chatInfo
meeting_info = MeetingInfo()
meetingInfo.@odatatype = '#microsoft.graph.organizerMeetingInfo'

meetingInfo.allow_conversation_without_host = True

additionalData = [
'organizer' => meeting_info = Organizer()
meetingInfo.@odatatype = '#microsoft.graph.identitySet'

user = User()
user.@odatatype = '#microsoft.graph.identity'

user.id = '5810cede-f3cc-42eb-b2c1-e9bd5d53ec96'

user.tenantId = 'aa67bd4c-8475-432d-bd41-39f255720e0a'

user.displayName = 'Bob'


meetingInfo.user = user

meetingInfo.organizer = organizer

];
meetingInfo.additionaldata(additionalData)



request_body.meeting_info = meetingInfo



result = await client.communications.calls.post(request_body = request_body)


```