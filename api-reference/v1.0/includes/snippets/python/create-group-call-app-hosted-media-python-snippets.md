---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Call();
requestBody.set@odatatype('#microsoft.graph.call');

requestBody.setDirection(CallDirection('outgoing'));

requestBody.setSubject('Create a group call with application hosted media');

requestBody.setCallbackUri('https://bot.contoso.com/callback');

source = ParticipantInfo();
source.set@odatatype('#microsoft.graph.participantInfo');

sourceIdentity = IdentitySet();
sourceIdentity.set@odatatype('#microsoft.graph.identitySet');

sourceIdentityApplication = Identity();
sourceIdentityApplication.set@odatatype('#microsoft.graph.identity');

sourceIdentityApplication.setDisplayName('TestBot');

sourceIdentityApplication.setId('dd3885da-f9ab-486b-bfae-85de3d445555');


sourceIdentity.setApplication($sourceIdentityApplication);

source.setIdentity($sourceIdentity);

requestBody.setSource($source);
targetsInvitationParticipantInfo1 = InvitationParticipantInfo();
targetsInvitationParticipantInfo1.set@odatatype('#microsoft.graph.invitationParticipantInfo');

targetsInvitationParticipantInfo1Identity = IdentitySet();
targetsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identitySet');

targetsInvitationParticipantInfo1IdentityUser = Identity();
targetsInvitationParticipantInfo1IdentityUser.set@odatatype('#microsoft.graph.identity');

targetsInvitationParticipantInfo1IdentityUser.setDisplayName('user1');

targetsInvitationParticipantInfo1IdentityUser.setId('98da8a1a-1b87-452c-a713-65d3f10b5555');


targetsInvitationParticipantInfo1Identity.setUser($targetsInvitationParticipantInfo1IdentityUser);

targetsInvitationParticipantInfo1.setIdentity($targetsInvitationParticipantInfo1Identity);

targetsArray []= targetsInvitationParticipantInfo1;
targetsInvitationParticipantInfo2 = InvitationParticipantInfo();
targetsInvitationParticipantInfo2.set@odatatype('#microsoft.graph.invitationParticipantInfo');

targetsInvitationParticipantInfo2Identity = IdentitySet();
targetsInvitationParticipantInfo2Identity.set@odatatype('#microsoft.graph.identitySet');

targetsInvitationParticipantInfo2IdentityUser = Identity();
targetsInvitationParticipantInfo2IdentityUser.set@odatatype('#microsoft.graph.identity');

targetsInvitationParticipantInfo2IdentityUser.setDisplayName('user2');

targetsInvitationParticipantInfo2IdentityUser.setId('bf5aae9a-d11d-47a8-93b1-782504c95555');


targetsInvitationParticipantInfo2Identity.setUser($targetsInvitationParticipantInfo2IdentityUser);

targetsInvitationParticipantInfo2.setIdentity($targetsInvitationParticipantInfo2Identity);

targetsArray []= targetsInvitationParticipantInfo2;
requestBody.setTargets(targetsArray);


requestBody.setRequestedModalities([requestBody.setModality(Modality('audio'));
]);

mediaConfig = MediaConfig();
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig');

additionalData = [
'removeFromDefaultAudioGroup' => false,
];
mediaConfig.setAdditionalData(additionalData);



requestBody.setMediaConfig($mediaConfig);


result = await client.communications().calls().post(requestBody);


```