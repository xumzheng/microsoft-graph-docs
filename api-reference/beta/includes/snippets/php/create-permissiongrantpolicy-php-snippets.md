---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PermissionGrantPolicy();


$requestRequestBody->setId('my-custom-consent-policy');
$requestRequestBody->setDisplayName('Custom application consent policy');
$requestRequestBody->setDescription('A custom permission grant policy to customize conditions for granting consent.');
$result =  $graphClient->policies()->permissionGrantPolicies()->post($requestRequestBody);


```