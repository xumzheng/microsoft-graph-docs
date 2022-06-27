---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ServicePrincipalIdsRequestBody();


$requestRequestBody->setServicePrincipalIds(['9089a539-a539-9089-39a5-899039a58990',]);
$result =  $graphClient->identityProtection()->riskyServicePrincipals()->confirmCompromised()->post($requestRequestBody);


```