---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new WorkforceIntegration();
$requestBody.setDisplayName('displayName-value');

$requestBody.setApiVersion(99);

$encryption = new WorkforceIntegrationEncryption();
$encryption.setProtocol(new WorkforceIntegrationEncryptionProtocol('protocol-value'));

$encryption.setSecret('secret-value');


$requestBody.setEncryption($encryption);
$requestBody.setIsActive(true);

$requestBody.setUrl('url-value');

$requestBody.setSupportedEntities(new WorkforceIntegrationSupportedEntities('supportedentities-value'));



$requestResult = $graphServiceClient.teamwork().workforceIntegrations().post($requestBody);


```