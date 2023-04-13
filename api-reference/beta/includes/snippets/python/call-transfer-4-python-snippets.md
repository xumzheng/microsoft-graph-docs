---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transfer_target = InvitationParticipantInfo()
transferTarget.@odatatype = '#microsoft.graph.invitationParticipantInfo'

transferTarget.EndpointType(EndpointType('default'))

transfer_target_identity = IdentitySet()
transferTargetIdentity.@odatatype = '#microsoft.graph.identitySet'

additionalData = [
'phone' => transfer_target_identity = Phone()
		transferTargetIdentity.@odatatype = '#microsoft.graph.identity'

		transferTargetIdentity.id = '+12345678901'


transferTargetIdentity.phone = phone

];
transferTargetIdentity.additionaldata(additionalData)



transferTarget.identity = transferTargetIdentity
transferTarget.replacesCallId = 'e5d39592-99bd-4db8-bca8-30fb894ec51d'

additionalData = [
'languageId' => 'en-us', 
'region' => 'amer', 
];
transferTarget.additionaldata(additionalData)



request_body.transfer_target = transferTarget



await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```