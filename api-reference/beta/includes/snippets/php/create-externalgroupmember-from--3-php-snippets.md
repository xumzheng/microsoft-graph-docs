---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Identity();


$requestRequestBody->setId('1431b9c38ee647f6a');
$requestRequestBody->setType(new IdentityType('externalGroup'));
$result =  $graphClient->external()->connectionsById('externalConnection-id')->groupsById('externalGroup-id')->members()->post($requestRequestBody);


```