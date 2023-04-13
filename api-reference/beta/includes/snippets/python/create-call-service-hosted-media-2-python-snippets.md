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

source_identity = IdentitySet()
sourceIdentity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'applicationInstance' => source_identity = ApplicationInstance()
		sourceIdentity.@odatatype = '#microsoft.graph.identity'

		sourceIdentity.displayName = 'Calling Bot'

		sourceIdentity.id = '3d913abb-aec0-4964-8fa6-3c6850c4f278'


sourceIdentity.application_instance = applicationInstance

];
sourceIdentity.additionaldata(additionalData)



source.identity = sourceIdentity
Source.countryCode=null

Source.endpointType=null

Source.region=null

Source.languageId=null


request_body.source = source
targets_invitation_participant_info1 = InvitationParticipantInfo()
targetsInvitationParticipantInfo1.@odatatype = '#microsoft.graph.invitationParticipantInfo'

targets_invitation_participant_info1_identity = IdentitySet()
targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'phone' => targets_invitation_participant_info1_identity = Phone()
		targetsInvitationParticipantInfo1Identity.@odatatype = '#microsoft.graph.identity'

		targetsInvitationParticipantInfo1Identity.id = '+12345678901'


targetsInvitationParticipantInfo1Identity.phone = phone

];
targetsInvitationParticipantInfo1Identity.additionaldata(additionalData)



targetsInvitationParticipantInfo1.identity = targetsInvitationParticipantInfo1Identity

targetsArray []= targetsInvitationParticipantInfo1;
request_body.targets(targetsArray)


request_body.RequestedModalities([request_body.Modality(Modality('audio'))
])

media_config = MediaConfig()
mediaConfig.@odatatype = '#microsoft.graph.serviceHostedMediaConfig'


request_body.media_config = mediaConfig
request_body.tenantId = 'aa67bd4c-8475-432d-bd41-39f255720e0a'




result = await client.communications.calls.post(request_body = request_body)


```