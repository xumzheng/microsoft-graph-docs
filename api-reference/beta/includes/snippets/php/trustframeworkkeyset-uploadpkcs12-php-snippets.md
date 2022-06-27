---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UploadPkcs12PostRequestBody();


$requestRequestBody->setKey('Base64-encoded-pfx-content');
$requestRequestBody->setPassword('password-value');
$result =  $graphClient->trustFramework()->keySetsById('trustFrameworkKeySet-id')->uploadPkcs12()->post($requestRequestBody);


```