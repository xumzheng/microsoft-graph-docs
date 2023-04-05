---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InvitePostRequestBody()
participantsInvitationParticipantInfo1 = InvitationParticipantInfo()
participantsInvitationParticipantInfo1.set@odatatype('#microsoft.graph.invitationParticipantInfo')

participantsInvitationParticipantInfo1Identity = IdentitySet()
participantsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identitySet')

additionalData = [
'phone' => participantsInvitationParticipantInfo1Identity = Phone()
		participantsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identity')

		participantsInvitationParticipantInfo1Identity.setId('+12345678901')


participantsInvitationParticipantInfo1Identity.setPhone($phone)

];
participantsInvitationParticipantInfo1Identity.setAdditionalData(additionalData)



participantsInvitationParticipantInfo1.setIdentity($participantsInvitationParticipantInfo1Identity)

participantsArray []= participantsInvitationParticipantInfo1;
request_body.setParticipants(participantsArray)


request_body.setClientContext('f2fa86af-3c51-4bc2-8fc0-475452d9764f')



result = await client.communications.callsby_id('call-id').participants.invite.post(request_body)


```