---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RedirectPostRequestBody()
targetsInvitationParticipantInfo1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.set@odatatype('#microsoft.graph.invitationParticipantInfo')

targetsInvitationParticipantInfo1Identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identitySet')

additionalData = [
'phone' => targetsInvitationParticipantInfo1Identity = Phone()
		targetsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identity')

		targetsInvitationParticipantInfo1Identity.setId('+12345678901')


targetsInvitationParticipantInfo1Identity.setPhone($phone)

];
targetsInvitationParticipantInfo1Identity.setAdditionalData(additionalData)



targetsInvitationParticipantInfo1.setIdentity($targetsInvitationParticipantInfo1Identity)

targetsArray []= targetsInvitationParticipantInfo1;
request_body.setTargets(targetsArray)


request_body.setCallbackUri('https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039')



await client.communications.calls._by_id('call-id').redirect.post(request_body)


```