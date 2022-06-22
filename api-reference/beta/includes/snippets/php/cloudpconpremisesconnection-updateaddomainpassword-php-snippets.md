---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AdDomainPasswordRequestBody();


$requestRequestBody->setAdDomainPassword('AdDomainPassword value');
$result =  $graphClient->deviceManagement()->virtualEndpoint()->onPremisesConnectionsById('cloudPcOnPremisesConnection-id')->updateAdDomainPassword()->post($requestRequestBody);


```