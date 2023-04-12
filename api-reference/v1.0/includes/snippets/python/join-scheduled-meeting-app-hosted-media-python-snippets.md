---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.Direction(CallDirection('outgoing'))

request_body.callbackUri = 'https://bot.contoso.com/callback'

request_body.RequestedModalities([request_body.Modality(Modality('audio'))
])

mediaConfig = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.appHostedMediaConfig'


request_body.mediaConfig = mediaConfig
chatInfo = ChatInfo()
chatInfo.@odatatype = '#microsoft.graph.chatInfo'

chatInfo.threadId = '19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2'

chatInfo.messageId = '0'


request_body.chatInfo = chatInfo
meetingInfo = MeetingInfo()
meetingInfo.@odatatype = '#microsoft.graph.organizerMeetingInfo'

additionalData = [
'organizer' => meetingInfo = Organizer()
	meetingInfo.@odatatype = '#microsoft.graph.identitySet'

user = User()
	user.@odatatype = '#microsoft.graph.identity'

	user.id = '5810cede-f3cc-42eb-b2c1-e9bd5d53ec96'

	user.tenantId = 'aa67bd4c-8475-432d-bd41-39f255720e0a'

	user.displayName = 'Bob'


meetingInfo.user = user

meetingInfo.organizer = organizer

'allowConversationWithoutHost' => true,
];
meetingInfo.additionaldata(additionalData)



request_body.meetingInfo = meetingInfo
request_body.tenantId = 'aa67bd4c-8475-432d-bd41-39f255720e0a'




result = await client.communications.calls.post(request_body = request_body)


```