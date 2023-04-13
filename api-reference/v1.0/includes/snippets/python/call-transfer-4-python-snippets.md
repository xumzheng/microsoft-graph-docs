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

additionalData = [
'phone' => transferTargetIdentity = Phone()
		transferTargetIdentity.@odatatype = '#microsoft.graph.identity'

		transferTargetIdentity.id = '+12345678901'


transferTargetIdentity.phone = phone

];
transferTargetIdentity.additionaldata(additionalData)



transferTarget.identity = transferTargetIdentity
transferTarget.replacesCallId = 'e5d39592-99bd-4db8-bca8-30fb894ec51d'

additionalData = [
'endpointType' => 'default', 
'languageId' => 'en-us', 
'region' => 'amer', 
];
transferTarget.additionaldata(additionalData)



request_body.transferTarget = transferTarget
additionalData = [
'clientContext' => '9e90d1c1-f61e-43e7-9f75-d420159aae08', 
];
request_body.additionaldata(additionalData)





await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```