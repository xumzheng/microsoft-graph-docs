---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.Direction(CallDirection('outgoing'))

request_body.subject = 'Create a group call with service hosted media'

request_body.callbackUri = 'https://bot.contoso.com/callback'

source = ParticipantInfo()
source.@odatatype = '#microsoft.graph.participantInfo'

source_identity = IdentitySet()
sourceIdentity.@odatatype = '#microsoft.graph.identitySet'

source_identity_application = Identity()
sourceIdentityApplication.@odatatype = '#microsoft.graph.identity'

sourceIdentityApplication.displayName = 'TestBot'

sourceIdentityApplication.id = 'dd3885da-f9ab-486b-bfae-85de3d445555'


sourceIdentity.application = sourceIdentityApplication

source.identity = sourceIdentity

request_body.source = source
targets_invitation_participant_info1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

targets_invitation_participant_info1_identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

targets_invitation_participant_info1_identity_user = Identity()
targetsInvitationParticipantInfo1IdentityUser.@odatatype = '#microsoft.graph.identity'

targetsInvitationParticipantInfo1IdentityUser.displayName = 'user1'

targetsInvitationParticipantInfo1IdentityUser.id = '98da8a1a-1b87-452c-a713-65d3f10b5555'


targetsInvitationParticipantInfo1Identity.user = targetsInvitationParticipantInfo1IdentityUser

targetsInvitationParticipantInfo1.identity = targetsInvitationParticipantInfo1Identity

targetsArray []= targetsInvitationParticipantInfo1;
targets_invitation_participant_info2 = InvitationParticipantInfo()
targetsInvitationParticipantInfo2.@odatatype = '#microsoft.graph.invitationParticipantInfo'

targets_invitation_participant_info2_identity = IdentitySet()
targetsInvitationParticipantInfo2Identity.@odatatype = '#microsoft.graph.identitySet'

targets_invitation_participant_info2_identity_user = Identity()
targetsInvitationParticipantInfo2IdentityUser.@odatatype = '#microsoft.graph.identity'

targetsInvitationParticipantInfo2IdentityUser.displayName = 'user2'

targetsInvitationParticipantInfo2IdentityUser.id = 'bf5aae9a-d11d-47a8-93b1-782504c95555'


targetsInvitationParticipantInfo2Identity.user = targetsInvitationParticipantInfo2IdentityUser

targetsInvitationParticipantInfo2.identity = targetsInvitationParticipantInfo2Identity

targetsArray []= targetsInvitationParticipantInfo2;
request_body.targets(targetsArray)


request_body.RequestedModalities([request_body.Modality(Modality('audio'))
])

media_config = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.serviceHostedMediaConfig'

additionalData = [
'removeFromDefaultAudioGroup' => false,
];
mediaConfig.additionaldata(additionalData)



request_body.media_config = mediaConfig



result = await client.communications.calls.post(request_body = request_body)


```