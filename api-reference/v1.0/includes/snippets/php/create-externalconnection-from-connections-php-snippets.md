---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalConnection();


$requestRequestBody->setId('contosohr');
$requestRequestBody->setName('Contoso HR');
$requestRequestBody->setDescription('Connection to index Contoso HR system');
$result =  $graphClient->external()->connections()->post($requestRequestBody);


```