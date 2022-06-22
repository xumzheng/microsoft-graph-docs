---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdentityProvider();


$requestRequestBody->setClientSecret('1111111111111');
$result =  $graphClient->identityProvidersById('identityProvider-id')->patch($requestRequestBody);


```