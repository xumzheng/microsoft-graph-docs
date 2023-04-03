---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = WorkforceIntegration();
requestBody.setDisplayName('displayName-value');

requestBody.setApiVersion(99);

encryption = WorkforceIntegrationEncryption();
encryption.setProtocol(WorkforceIntegrationEncryptionProtocol('protocol-value'));

encryption.setSecret('secret-value');


requestBody.setEncryption($encryption);
requestBody.setIsActive(true);

requestBody.setUrl('url-value');

requestBody.setSupportedEntities(WorkforceIntegrationSupportedEntities('supportedentities-value'));



result = await client.teamwork().workforceIntegrations().post(requestBody);


```