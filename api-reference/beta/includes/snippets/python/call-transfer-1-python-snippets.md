---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transfer_target = InvitationParticipantInfo()
transferTarget.EndpointType(EndpointType('default'))

transfer_target_identity = IdentitySet()
transfer_target_identity_user = Identity()
transferTargetIdentityUser.id = '550fae72-d251-43ec-868c-373732c2704f'

transferTargetIdentityUser.displayName = 'Heidi Steen'

additionalData = [
'tenantId' => '72f988bf-86f1-41af-91ab-2d7cd011db47', 
];
transferTargetIdentityUser.additionaldata(additionalData)



transferTargetIdentity.user = transferTargetIdentityUser

transferTarget.identity = transferTargetIdentity
additionalData = [
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.additionaldata(additionalData)



request_body.transfer_target = transferTarget



await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```