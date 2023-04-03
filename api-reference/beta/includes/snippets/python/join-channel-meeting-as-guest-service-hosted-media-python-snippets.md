---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Call();
requestBody.set@odatatype('#microsoft.graph.call');

requestBody.setCallbackUri('https://bot.contoso.com/callback');

source = ParticipantInfo();
source.set@odatatype('#microsoft.graph.participantInfo');

sourceIdentity = IdentitySet();
sourceIdentity.set@odatatype('#microsoft.graph.identitySet');

additionalData = [
'guest' => sourceIdentity = Guest();
		sourceIdentity.set@odatatype('#microsoft.graph.identity');

		sourceIdentity.setDisplayName('Guest User');

		sourceIdentity.setId('d7a3b999-17ac-4bca-9e77-e6a730d2ec2e');


sourceIdentity.setGuest($guest);

];
sourceIdentity.setAdditionalData(additionalData);



source.setIdentity($sourceIdentity);

requestBody.setSource($source);
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

chatInfo.setThreadId('19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype');

chatInfo.setMessageId('1533758867081');


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


result = awaitclient.communications().calls().post(requestBody);


```