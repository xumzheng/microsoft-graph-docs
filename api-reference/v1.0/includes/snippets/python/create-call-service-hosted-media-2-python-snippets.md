---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Call()
request_body.set@odatatype('#microsoft.graph.call')

request_body.setCallbackUri('https://bot.contoso.com/callback')

source = ParticipantInfo()
source.set@odatatype('#microsoft.graph.participantInfo')

sourceIdentity = IdentitySet()
sourceIdentity.set@odatatype('#microsoft.graph.identitySet')

additionalData = [
'applicationInstance' => sourceIdentity = ApplicationInstance()
		sourceIdentity.set@odatatype('#microsoft.graph.identity')

		sourceIdentity.setDisplayName('Calling Bot')

		sourceIdentity.setId('3d913abb-aec0-4964-8fa6-3c6850c4f278')


sourceIdentity.setApplicationInstance($applicationInstance)

];
sourceIdentity.setAdditionalData(additionalData)



source.setIdentity($sourceIdentity)
Source.setCountryCode(null)

Source.setEndpointType(null)

Source.setRegion(null)

Source.setLanguageId(null)


request_body.setSource($source)
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


request_body.setRequestedModalities([request_body.setModality(Modality('audio'))
])

mediaConfig = MediaConfig()
mediaConfig.set@odatatype('#microsoft.graph.serviceHostedMediaConfig')


request_body.setMediaConfig($mediaConfig)
request_body.setTenantId('aa67bd4c-8475-432d-bd41-39f255720e0a')



result = await client.communications.calls.post(request_body)


```