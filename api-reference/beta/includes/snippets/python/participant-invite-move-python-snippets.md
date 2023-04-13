---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InvitePostRequestBody()
participants_invitation_participant_info1 = InvitationParticipantInfo()
participantsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

participantsInvitationParticipantInfo1.replacesCallId = 'a7ebfb2d-871e-419c-87af-27290b22e8db'

participantsInvitationParticipantInfo1.participantId = '7d501bf1-5ee4-4605-ba92-0ae4513c611c'

participants_invitation_participant_info1_identity = IdentitySet()
participantsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

participants_invitation_participant_info1_identity_user = Identity()
participantsInvitationParticipantInfo1IdentityUser.@odatatype = '#microsoft.graph.identity'

participantsInvitationParticipantInfo1IdentityUser.id = '682b6c37-0729-4fab-ace6-d730d5d9137e'

additionalData = [
'identityProvider' => 'AAD', 
];
participantsInvitationParticipantInfo1IdentityUser.additionaldata(additionalData)



participantsInvitationParticipantInfo1Identity.user = participantsInvitationParticipantInfo1IdentityUser

participantsInvitationParticipantInfo1.identity = participantsInvitationParticipantInfo1Identity

participantsArray []= participantsInvitationParticipantInfo1;
request_body.participants(participantsArray)


request_body.clientContext = 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'




result = await client.communications.calls_by_id('call-id').participants.invite.post(request_body = request_body)


```