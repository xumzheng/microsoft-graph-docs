---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.@odatatype = '#microsoft.graph.call'

request_body.callbackUri = 'https://bot.contoso.com/callback'

source = ParticipantInfo()
source.@odatatype = '#microsoft.graph.participantInfo'

sourceIdentity = IdentitySet()
sourceIdentity.@odatatype = '#microsoft.graph.identitySet'

sourceIdentityApplication = Identity()
sourceIdentityApplication.@odatatype = '#microsoft.graph.identity'

sourceIdentityApplication.displayName = 'Calling Bot'

sourceIdentityApplication.id = '2891555a-92ff-42e6-80fa-6e1300c6b5c6'


sourceIdentity.application = sourceIdentityApplication

source.identity = sourceIdentity
Source.region=null

Source.languageId=null


request_body.source = source
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

mediaConfig = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.appHostedMediaConfig'

additionalData = [
'blob' => '<Media Session Configuration>', 
];
mediaConfig.additionaldata(additionalData)



request_body.mediaConfig = mediaConfig



result = await client.communications.calls.post(request_body = request_body)


```