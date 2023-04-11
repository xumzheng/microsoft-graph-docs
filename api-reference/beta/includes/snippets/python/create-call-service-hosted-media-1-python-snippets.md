---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.callbackUri = 'https://bot.contoso.com/callback'

targetsInvitationParticipantInfo1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

targetsInvitationParticipantInfo1Identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

targetsInvitationParticipantInfo1IdentityUser = Identity()
targetsInvitationParticipantInfo1IdentityUser.@odatatype = '#microsoft.graph.identity'

targetsInvitationParticipantInfo1IdentityUser.displayName = 'John'

targetsInvitationParticipantInfo1IdentityUser.id = '112f7296-5fa4-42ca-bae8-6a692b15d4b8'


targetsInvitationParticipantInfo1Identity.user = targetsInvitationParticipantInfo1IdentityUser

targetsInvitationParticipantInfo1.identity = targetsInvitationParticipantInfo1Identity

targetsArray []= targetsInvitationParticipantInfo1;
request_body.targets(targetsArray)


request_body.RequestedModalities([request_body.Modality(Modality('audio'))
])

callOptions = CallOptions()
callOptions.@odatatype = '#microsoft.graph.outgoingCallOptions'

callOptions.isContentSharingNotificationEnabled = true


request_body.callOptions = callOptions
mediaConfig = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.serviceHostedMediaConfig'


request_body.mediaConfig = mediaConfig


request_configuration = CallsRequestBuilderPostRequestConfiguration(
)


result = await client.communications.calls.post(request_body = request_body)


```