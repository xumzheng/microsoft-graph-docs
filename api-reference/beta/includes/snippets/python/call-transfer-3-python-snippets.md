---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transferTarget = InvitationParticipantInfo()
transferTarget.EndpointType(EndpointType('default'))

transferTargetIdentity = IdentitySet()
additionalData = [
'phone' => transferTargetIdentity = Phone()
		transferTargetIdentity.@odatatype = '#microsoft.graph.identity'

		transferTargetIdentity.id = '+12345678901'


transferTargetIdentity.phone = phone

];
transferTargetIdentity.additionaldata(additionalData)



transferTarget.identity = transferTargetIdentity
additionalData = [
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.additionaldata(additionalData)



request_body.transferTarget = transferTarget



await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```