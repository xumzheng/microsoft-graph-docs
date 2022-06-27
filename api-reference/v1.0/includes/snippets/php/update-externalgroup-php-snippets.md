---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalGroup();


$requestRequestBody->setDisplayName('Contoso Marketing');
$requestRequestBody->setDescription('The product marketing team');
$result =  $graphClient->external()->connectionsById('externalConnection-id')->groupsById('externalGroup-id')->patch($requestRequestBody);


```