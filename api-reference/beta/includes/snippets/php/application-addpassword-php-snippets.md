---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PasswordCredentialRequestBody();



$passwordCredential = new PasswordCredential();
$requestRequestBody->setPasswordCredential($passwordCredential);


$passwordCredential->setDisplayName('Password friendly name');

$result =  $graphClient->applicationsById('application-id')->addPassword()->post($requestRequestBody);


```