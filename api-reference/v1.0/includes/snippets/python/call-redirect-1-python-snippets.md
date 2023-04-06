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

targetsInvitationParticipantInfo1IdentityApplication = Identity()
targetsInvitationParticipantInfo1IdentityApplication.set@odatatype('#microsoft.graph.identity')

targetsInvitationParticipantInfo1IdentityApplication.setDisplayName('test bot 2')

targetsInvitationParticipantInfo1IdentityApplication.setId('22bfd41f-550e-477d-8789-f6f7bd2a5e8b')


targetsInvitationParticipantInfo1Identity.setApplication($targetsInvitationParticipantInfo1IdentityApplication)

targetsInvitationParticipantInfo1.setIdentity($targetsInvitationParticipantInfo1Identity)

targetsArray []= targetsInvitationParticipantInfo1;
request_body.setTargets(targetsArray)


request_body.setCallbackUri('https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039')



await client.communications.calls_by_id('call-id').redirect.post(request_body, headers=)


```