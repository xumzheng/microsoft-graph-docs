---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Call();
request_body.set@odatatype('#microsoft.graph.call');

request_body.setDirection(CallDirection('outgoing'));

request_body.setCallbackUri('https://bot.contoso.com/callback');

request_body.setRequestedModalities([request_body.setModality(Modality('audio'));
]);

mediaConfig = MediaConfig();
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig');


request_body.setMediaConfig($mediaConfig);
chatInfo = ChatInfo();
chatInfo.set@odatatype('#microsoft.graph.chatInfo');

chatInfo.setThreadId('19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2');

chatInfo.setMessageId('0');


request_body.setChatInfo($chatInfo);
meetingInfo = MeetingInfo();
meetingInfo.set@odatatype('#microsoft.graph.organizerMeetingInfo');

additionalData = [
'organizer' => meetingInfo = Organizer();
	meetingInfo.set@odatatype('#microsoft.graph.identitySet');

user = User();
	user.set@odatatype('#microsoft.graph.identity');

	user.setId('5810cede-f3cc-42eb-b2c1-e9bd5d53ec96');

	user.setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a');

	user.setDisplayName('Bob');


meetingInfo.setUser($user);

meetingInfo.setOrganizer($organizer);

'allowConversationWithoutHost' => true,
];
meetingInfo.setAdditionalData(additionalData);



request_body.setMeetingInfo($meetingInfo);
request_body.setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a');



result = await client.communications.calls.post(request_body);


```