---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AppRoleAssignment();


$requestRequestBody->setPrincipalId('9028d19c-26a9-4809-8e3f-20ff73e2d75e');
$requestRequestBody->setResourceId('8fce32da-1246-437b-99cd-76d1d4677bd5');
$requestRequestBody->setAppRoleId('498476ce-e0fe-48b0-b801-37ba7e2685c6');
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->appRoleAssignments()->post($requestRequestBody);


```