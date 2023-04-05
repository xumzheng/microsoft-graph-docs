---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transferTarget = InvitationParticipantInfo()
transferTarget.set@odatatype('#microsoft.graph.invitationParticipantInfo')

transferTarget.setEndpointType(EndpointType('default'))

transferTargetIdentity = IdentitySet()
transferTargetIdentity.set@odatatype('#microsoft.graph.identitySet')

transferTargetIdentityUser = Identity()
transferTargetIdentityUser.set@odatatype('#microsoft.graph.identity')

transferTargetIdentityUser.setId('550fae72-d251-43ec-868c-373732c2704f')

transferTargetIdentityUser.setDisplayName('Heidi Steen')

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transferTargetIdentityUser.setAdditionalData(additionalData)



transferTargetIdentity.setUser($transferTargetIdentityUser)

transferTarget.setIdentity($transferTargetIdentity)
transferTarget.setReplacesCallId('e5d39592-99bd-4db8-bca8-30fb894ec51d')

additionalData = [
'languageId' => 'en-us', 
'region' => 'amer', 
];
transferTarget.setAdditionalData(additionalData)



request_body.setTransferTarget($transferTarget)


await client.communications.callsById('call-id').transfer.post(request_body)


```