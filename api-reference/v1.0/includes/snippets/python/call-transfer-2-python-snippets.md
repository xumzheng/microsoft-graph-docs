---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transferTarget = InvitationParticipantInfo()
transferTarget.@odatatype = '#microsoft.graph.invitationParticipantInfo'

transferTargetIdentity = IdentitySet()
transferTargetIdentity.@odatatype = '#microsoft.graph.identitySet'

transferTargetIdentityUser = Identity()
transferTargetIdentityUser.@odatatype = '#microsoft.graph.identity'

transferTargetIdentityUser.id = '550fae72-d251-43ec-868c-373732c2704f'

transferTargetIdentityUser.displayName = 'Heidi Steen'


transferTargetIdentity.user = transferTargetIdentityUser

transferTarget.identity = transferTargetIdentity
transferTarget.replacesCallId = 'e5d39592-99bd-4db8-bca8-30fb894ec51d'

additionalData = [
'endpointType' => 'default', 
];
transferTarget.additionaldata(additionalData)



request_body.transferTarget = transferTarget



await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```