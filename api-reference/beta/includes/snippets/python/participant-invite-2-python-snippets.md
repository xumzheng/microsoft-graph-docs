---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InvitePostRequestBody()
participantsInvitationParticipantInfo1 = InvitationParticipantInfo()
participantsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

participantsInvitationParticipantInfo1Identity = IdentitySet()
participantsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'phone' => participantsInvitationParticipantInfo1Identity = Phone()
		participantsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identity'

		participantsInvitationParticipantInfo1Identity.id = '+12345678901'


participantsInvitationParticipantInfo1Identity.phone = phone

];
participantsInvitationParticipantInfo1Identity.additionaldata(additionalData)



participantsInvitationParticipantInfo1.identity = participantsInvitationParticipantInfo1Identity

participantsArray []= participantsInvitationParticipantInfo1;
request_body.participants(participantsArray)


request_body.clientContext = 'f2fa86af-3c51-4bc2-8fc0-475452d9764f'



request_configuration = InviteRequestBuilderPostRequestConfiguration(
)


result = await client.communications.calls_by_id('call-id').participants.invite.post(request_body = request_body)


```