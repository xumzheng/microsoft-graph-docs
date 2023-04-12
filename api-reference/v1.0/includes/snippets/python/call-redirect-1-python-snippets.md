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

targetsInvitationParticipantInfo1IdentityApplication = Identity()
targetsInvitationParticipantInfo1IdentityApplication.@odatatype = '#microsoft.graph.identity'

targetsInvitationParticipantInfo1IdentityApplication.displayName = 'test bot 2'

targetsInvitationParticipantInfo1IdentityApplication.id = '22bfd41f-550e-477d-8789-f6f7bd2a5e8b'


targetsInvitationParticipantInfo1Identity.application = targetsInvitationParticipantInfo1IdentityApplication

targetsInvitationParticipantInfo1.identity = targetsInvitationParticipantInfo1Identity

targetsArray []= targetsInvitationParticipantInfo1;
request_body.targets(targetsArray)


request_body.callbackUri = 'https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039'




await client.communications.calls_by_id('call-id').redirect.post(request_body = request_body)


```