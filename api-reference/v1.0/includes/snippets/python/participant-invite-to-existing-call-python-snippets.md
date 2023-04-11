---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InvitePostRequestBody()
participantsInvitationParticipantInfo1 = InvitationParticipantInfo()
participantsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

participantsInvitationParticipantInfo1.replacesCallId = 'a7ebfb2d-871e-419c-87af-27290b22e8db'

participantsInvitationParticipantInfo1Identity = IdentitySet()
participantsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

participantsInvitationParticipantInfo1IdentityUser = Identity()
participantsInvitationParticipantInfo1IdentityUser.@odatatype = '#microsoft.graph.identity'

participantsInvitationParticipantInfo1IdentityUser.id = '278405a3-f568-4b3e-b684-009193463064'

participantsInvitationParticipantInfo1IdentityUser.displayName = 'string'


participantsInvitationParticipantInfo1Identity.user = participantsInvitationParticipantInfo1IdentityUser

participantsInvitationParticipantInfo1.identity = participantsInvitationParticipantInfo1Identity

participantsArray []= participantsInvitationParticipantInfo1;
request_body.participants(participantsArray)


request_body.clientContext = 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'




result = await client.communications.calls_by_id('call-id').participants.invite.post(request_body = request_body)


```