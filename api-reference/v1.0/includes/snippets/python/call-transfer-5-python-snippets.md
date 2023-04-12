---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transferTarget = InvitationParticipantInfo()
transferTargetIdentity = IdentitySet()
transferTargetIdentityUser = Identity()
transferTargetIdentityUser.id = '550fae72-d251-43ec-868c-373732c2704f'

transferTargetIdentityUser.displayName = 'Heidi Steen'


transferTargetIdentity.user = transferTargetIdentityUser

transferTarget.identity = transferTargetIdentity
additionalData = [
'endpointType' => 'default', 
];
transferTarget.additionaldata(additionalData)



request_body.transferTarget = transferTarget
transferee = ParticipantInfo()
transfereeIdentity = IdentitySet()
transfereeIdentityUser = Identity()
transfereeIdentityUser.id = '751f6800-3180-414d-bd94-333364659951'

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transfereeIdentityUser.additionaldata(additionalData)



transfereeIdentity.user = transfereeIdentityUser

transferee.identity = transfereeIdentity
transferee.participantId = '909c6581-5130-43e9-88f3-fcb3582cde37'


request_body.transferee = transferee



await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```