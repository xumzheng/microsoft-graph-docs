---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Permission();


$requestRequestBody->setRoles( [
'write',],
$grantedToIdentitiesArray = [];

$grantedToIdentities1 = new IdentitySet();


$application = new Identity();
$grantedToIdentities1->setApplication($application);


$application->setId('89ea5c94-7736-4e25-95ad-3fa95f62b66e');
$application->setDisplayName('Contoso Time Manager App');


$grantedToIdentitiesArray []= $grantedToIdentities1;
$requestRequestBody->setGrantedToIdentities($grantedToIdentitiesArray);
$result =  $graphClient->sitesById('site-id')->permissions()->post($requestRequestBody);


```