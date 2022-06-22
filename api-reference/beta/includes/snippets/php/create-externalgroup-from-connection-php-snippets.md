---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalGroup();


$requestRequestBody->setId('31bea3d537902000');
$requestRequestBody->setDisplayName('Contoso Marketing');
$requestRequestBody->setDescription('The product marketing team');
$result =  $graphClient->external()->connectionsById('externalConnection-id')->groups()->post($requestRequestBody);


```