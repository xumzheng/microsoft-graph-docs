---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RedirectPostRequestBody()
targetsInvitationParticipantInfo1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

targetsInvitationParticipantInfo1Identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'phone' => targetsInvitationParticipantInfo1Identity = Phone()
		targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identity'

		targetsInvitationParticipantInfo1Identity.id = '+12345678901'


targetsInvitationParticipantInfo1Identity.phone = phone

];
targetsInvitationParticipantInfo1Identity.additionaldata(additionalData)



targetsInvitationParticipantInfo1.identity = targetsInvitationParticipantInfo1Identity

targetsArray []= targetsInvitationParticipantInfo1;
request_body.targets(targetsArray)


request_body.callbackUri = 'https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039'



request_configuration = RedirectRequestBuilderPostRequestConfiguration(
)


await client.communications.calls_by_id('call-id').redirect.post(request_body = request_body)


```