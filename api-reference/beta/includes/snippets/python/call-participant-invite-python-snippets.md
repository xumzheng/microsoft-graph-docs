---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = InvitePostRequestBody();
participantsInvitationParticipantInfo1 = InvitationParticipantInfo();
participantsInvitationParticipantInfo1.set@odatatype('#microsoft.graph.invitationParticipantInfo');

participantsInvitationParticipantInfo1.setReplacesCallId('a7ebfb2d-871e-419c-87af-27290b22e8db');

participantsInvitationParticipantInfo1Identity = IdentitySet();
participantsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identitySet');

participantsInvitationParticipantInfo1IdentityUser = Identity();
participantsInvitationParticipantInfo1IdentityUser.set@odatatype('#microsoft.graph.identity');

participantsInvitationParticipantInfo1IdentityUser.setId('278405a3-f568-4b3e-b684-009193463064');

additionalData = [
'identityProvider' => 'AAD', 
];
participantsInvitationParticipantInfo1IdentityUser.setAdditionalData(additionalData);



participantsInvitationParticipantInfo1Identity.setUser($participantsInvitationParticipantInfo1IdentityUser);

participantsInvitationParticipantInfo1.setIdentity($participantsInvitationParticipantInfo1Identity);

participantsArray []= participantsInvitationParticipantInfo1;
request_body.setParticipants(participantsArray);


request_body.setClientContext('f2fa86af-3c51-4bc2-8fc0-475452d9764f');



result = await client.communications().callsById('call-id').participants().invite().post(request_body);


```