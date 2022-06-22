---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Identity();


$requestRequestBody->setId('e811976d-83df-4cbd-8b9b-5215b18aa874');
$requestRequestBody->setType(new IdentityType('user'));
$result =  $graphClient->external()->connectionsById('externalConnection-id')->groupsById('externalGroup-id')->members()->post($requestRequestBody);


```