---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DelegatedPermissionClassification();


$requestRequestBody->setPermissionId('e1fe6dd8-ba31-4d61-89e7-88639da4683d');
$requestRequestBody->setPermissionName('User.Read');
$requestRequestBody->setClassification(new PermissionClassificationType('low'));
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->delegatedPermissionClassifications()->post($requestRequestBody);


```