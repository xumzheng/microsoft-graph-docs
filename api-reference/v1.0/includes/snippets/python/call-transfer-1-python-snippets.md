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
transferTargetIdentityUser.setId('550fae72-d251-43ec-868c-373732c2704f')

transferTargetIdentityUser.setDisplayName('Heidi Steen')


transferTargetIdentity.setUser($transferTargetIdentityUser)

transferTarget.setIdentity($transferTargetIdentity)
additionalData = [
'endpointType' => 'default', 
];
transferTarget.setAdditionalData(additionalData)



request_body.setTransferTarget($transferTarget)


await client.communications.calls._by_id('call-id').transfer.post(request_body)


```