---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrintTaskDefinition();


$requestRequestBody->setDisplayName('Test TaskDefinitionName');

$createdBy = new AppIdentity();
$requestRequestBody->setCreatedBy($createdBy);


$createdBy->setDisplayName('Requesting App Display Name');

$result =  $graphClient->print()->taskDefinitions()->post($requestRequestBody);


```