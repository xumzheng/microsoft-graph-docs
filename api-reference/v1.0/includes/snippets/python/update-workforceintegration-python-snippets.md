---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkforceIntegration()
request_body.displayName = 'displayName-value'

request_body.apiVersion = 99

encryption = WorkforceIntegrationEncryption()
encryption.Protocol(WorkforceIntegrationEncryptionProtocol('protocol-value'))

encryption.secret = 'secret-value'


request_body.encryption = encryption
request_body.isActive = true

request_body.url = 'url-value'

request_body.SupportedEntities(WorkforceIntegrationSupportedEntities('supportedentities-value'))



request_configuration = WorkforceIntegrationRequestBuilderPatchRequestConfiguration(
)


result = await client.teamwork.workforceIntegrations_by_id('workforceIntegration-id').patch(request_body = request_body)


```