---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Call();
requestBody.set@odatatype('#microsoft.graph.call');

requestBody.setDirection(CallDirection('outgoing'));

requestBody.setCallbackUri('https://bot.contoso.com/callback');

requestBody.setRequestedModalities([requestBody.setModality(Modality('audio'));
]);

mediaConfig = MediaConfig();
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig');

additionalData = [
'blob' => '<Media Session Configuration>', 
];
mediaConfig.setAdditionalData(additionalData);



requestBody.setMediaConfig($mediaConfig);
chatInfo = ChatInfo();
chatInfo.set@odatatype('#microsoft.graph.chatInfo');

chatInfo.setThreadId('19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2');

chatInfo.setMessageId('0');


requestBody.setChatInfo($chatInfo);
meetingInfo = MeetingInfo();
meetingInfo.set@odatatype('#microsoft.graph.organizerMeetingInfo');

meetingInfo.setAllowConversationWithoutHost(true);

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

];
meetingInfo.setAdditionalData(additionalData);



requestBody.setMeetingInfo($meetingInfo);
requestBody.setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a');



requestResult = graphServiceClient.communications().calls().post(requestBody);


```