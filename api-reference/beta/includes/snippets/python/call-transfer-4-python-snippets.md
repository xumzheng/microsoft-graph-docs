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

additionalData = [
'phone' => transferTargetIdentity = Phone()
		transferTargetIdentity.set@odatatype('#microsoft.graph.identity')

		transferTargetIdentity.setId('+12345678901')


transferTargetIdentity.setPhone($phone)

];
transferTargetIdentity.setAdditionalData(additionalData)



transferTarget.setIdentity($transferTargetIdentity)
transferTarget.setReplacesCallId('e5d39592-99bd-4db8-bca8-30fb894ec51d')

additionalData = [
'languageId' => 'en-us', 
'region' => 'amer', 
];
transferTarget.setAdditionalData(additionalData)



request_body.setTransferTarget($transferTarget)


await client.communications.calls_by_id('call-id').transfer.post(request_body)


```