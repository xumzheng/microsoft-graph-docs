---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.set@odatatype('#microsoft.graph.call')

request_body.setCallbackUri('https://bot.contoso.com/callback')

targetsInvitationParticipantInfo1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.set@odatatype('#microsoft.graph.invitationParticipantInfo')

targetsInvitationParticipantInfo1Identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.set@odatatype('#microsoft.graph.identitySet')

targetsInvitationParticipantInfo1IdentityUser = Identity()
targetsInvitationParticipantInfo1IdentityUser.set@odatatype('#microsoft.graph.identity')

targetsInvitationParticipantInfo1IdentityUser.setDisplayName('John')

targetsInvitationParticipantInfo1IdentityUser.setId('112f7296-5fa4-42ca-bae8-6a692b15d4b8')


targetsInvitationParticipantInfo1Identity.setUser($targetsInvitationParticipantInfo1IdentityUser)

targetsInvitationParticipantInfo1.setIdentity($targetsInvitationParticipantInfo1Identity)

targetsArray []= targetsInvitationParticipantInfo1;
request_body.setTargets(targetsArray)


request_body.setRequestedModalities([request_body.setModality(Modality('audio'))
])

callOptions = CallOptions()
callOptions.set@odatatype('#microsoft.graph.outgoingCallOptions')

callOptions.setIsContentSharingNotificationEnabled(true)


request_body.setCallOptions($callOptions)
mediaConfig = MediaConfig()
mediaConfig.set@odatatype('#microsoft.graph.serviceHostedMediaConfig')


request_body.setMediaConfig($mediaConfig)


result = await client.communications.calls.post(request_body)


```