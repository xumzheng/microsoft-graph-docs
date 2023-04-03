---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Call();
requestBody.set@odatatype('#microsoft.graph.call');

requestBody.setCallbackUri('https://bot.contoso.com/callback');

requestBody.setRequestedModalities([requestBody.setModality(Modality('audio'));
]);

mediaConfig = MediaConfig();
mediaConfig.set@odatatype('#microsoft.graph.serviceHostedMediaConfig');

additionalData = [
'preFetchMedia' => preFetchMedia1 = ();
	preFetchMedia1.setUri('https://cdn.contoso.com/beep.wav');

	preFetchMedia1.setResourceId('f8971b04-b53e-418c-9222-c82ce681a582');


preFetchMediaArray []= preFetchMedia1;
preFetchMedia2 = ();
	preFetchMedia2.setUri('https://cdn.contoso.com/cool.wav');

	preFetchMedia2.setResourceId('86dc814b-c172-4428-9112-60f8ecae1edb');


preFetchMediaArray []= preFetchMedia2;
mediaConfig.setPreFetchMedia(preFetchMediaArray);


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

additionalData = [
'organizer' => meetingInfo = Organizer();
meetingInfo.set@odatatype('#microsoft.graph.identitySet');

user = User();
user.set@odatatype('#microsoft.graph.identity');

user.setId('5810cede-f3cc-42eb-b2c1-e9bd5d53ec96');

user.setDisplayName('Bob');

user.setTenantId('86dc81db-c112-4228-9222-63f3esaa1edb');


meetingInfo.setUser($user);

meetingInfo.setOrganizer($organizer);

'allowConversationWithoutHost' => true,
];
meetingInfo.setAdditionalData(additionalData);



requestBody.setMeetingInfo($meetingInfo);
requestBody.setTenantId('86dc81db-c112-4228-9222-63f3esaa1edb');



requestResult = graphServiceClient.communications().calls().post(requestBody);


```