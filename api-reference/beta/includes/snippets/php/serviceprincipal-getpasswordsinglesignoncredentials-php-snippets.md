---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new IdRequestBody();


$requestRequestBody->setId('5793aa3b-cca9-4794-679a240f8b58');
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->getPasswordSingleSignOnCredentials()->post($requestRequestBody);


```