---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TransferPostRequestBody()
transfer_target = InvitationParticipantInfo()
transfer_target_identity = IdentitySet()
additionalData = [
'phone' => transfer_target_identity = Phone()
		transferTargetIdentity.@odatatype = '#microsoft.graph.identity'

		transferTargetIdentity.id = '+12345678901'


transferTargetIdentity.phone = phone

];
transferTargetIdentity.additionaldata(additionalData)



transferTarget.identity = transferTargetIdentity
additionalData = [
'endpointType' => 'default', 
'languageId' => 'languageId-value', 
'region' => 'region-value', 
];
transferTarget.additionaldata(additionalData)



request_body.transfer_target = transferTarget
additionalData = [
'clientContext' => '9e90d1c1-f61e-43e7-9f75-d420159aae08', 
];
request_body.additionaldata(additionalData)





await client.communications.calls_by_id('call-id').transfer.post(request_body = request_body)


```