---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AddTokenSigningCertificatePostRequestBody();


$requestRequestBody->setDisplayName('CN=customDisplayName');
$requestRequestBody->setEndDateTime(new DateTime("2024-01-25T00:00:00Z"));
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->addTokenSigningCertificate()->post($requestRequestBody);


```