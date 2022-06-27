---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Identity();


$requestRequestBody->setId('e5477431-1038-484e-bf69-1dfedb97a110');
$requestRequestBody->setType(new IdentityType('externalGroup'));
$result =  $graphClient->external()->connectionsById('externalConnection-id')->groupsById('externalGroup-id')->members()->post($requestRequestBody);


```