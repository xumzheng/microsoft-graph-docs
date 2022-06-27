---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AppRoleAssignment();


$requestRequestBody->setPrincipalId('33ad69f9-da99-4bed-acd0-3f24235cb296');
$requestRequestBody->setResourceId('9028d19c-26a9-4809-8e3f-20ff73e2d75e');
$requestRequestBody->setAppRoleId('ef7437e6-4f94-4a0a-a110-a439eb2aa8f7');
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->appRoleAssignedTo()->post($requestRequestBody);


```