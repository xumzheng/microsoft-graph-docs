---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WorkforceIntegration();


$requestRequestBody->setDisplayName('displayName-value');
$requestRequestBody->setApiVersion(99);

$encryption = new WorkforceIntegrationEncryption();
$requestRequestBody->setEncryption($encryption);


$encryption->setProtocol(new WorkforceIntegrationEncryptionProtocol('protocol-value'));
$encryption->setSecret('secret-value');

$requestRequestBody->setIsActive(True);
$requestRequestBody->setUrl('url-value');
$requestRequestBody->setSupportedEntities(new WorkforceIntegrationSupportedEntities('supportedEntities-value'));
$result =  $graphClient->teamwork()->workforceIntegrations()->post($requestRequestBody);


```