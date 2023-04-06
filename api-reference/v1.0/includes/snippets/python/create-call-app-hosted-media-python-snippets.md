---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Call()
request_body.set@odatatype('#microsoft.graph.call')

request_body.setCallbackUri('https://bot.contoso.com/callback')

source = ParticipantInfo()
source.set@odatatype('#microsoft.graph.participantInfo')

sourceIdentity = IdentitySet()
sourceIdentity.set@odatatype('#microsoft.graph.identitySet')

sourceIdentityApplication = Identity()
sourceIdentityApplication.set@odatatype('#microsoft.graph.identity')

sourceIdentityApplication.setDisplayName('Calling Bot')

sourceIdentityApplication.setId('2891555a-92ff-42e6-80fa-6e1300c6b5c6')


sourceIdentity.setApplication($sourceIdentityApplication)

source.setIdentity($sourceIdentity)
Source.setRegion(null)

Source.setLanguageId(null)


request_body.setSource($source)
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

mediaConfig = MediaConfig()
mediaConfig.set@odatatype('#microsoft.graph.appHostedMediaConfig')

additionalData = [
'blob' => '<Media Session Configuration>', 
];
mediaConfig.setAdditionalData(additionalData)



request_body.setMediaConfig($mediaConfig)

request_config = CallsRequestBuilderPostRequestConfiguration(
request_config = CallsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.communications.calls.post(request_body, headers=)


```