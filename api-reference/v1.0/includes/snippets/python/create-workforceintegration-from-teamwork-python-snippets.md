---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkforceIntegration()
request_body.setDisplayName('displayName-value')

request_body.setApiVersion(99)

encryption = WorkforceIntegrationEncryption()
encryption.setProtocol(WorkforceIntegrationEncryptionProtocol('protocol-value'))

encryption.setSecret('secret-value')


request_body.setEncryption($encryption)
request_body.setIsActive(true)

request_body.setUrl('url-value')

request_body.setSupportedEntities(WorkforceIntegrationSupportedEntities('supportedentities-value'))


request_config = WorkforceIntegrationsRequestBuilderPostRequestConfiguration(
request_config = WorkforceIntegrationsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teamwork.workforceIntegrations.post(request_body, headers=)


```