---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ExternalConnection();


$requestRequestBody->setName('Contoso HR Service Tickets');
$requestRequestBody->setDescription('Connection to index HR service tickets');
$result =  $graphClient->external()->connectionsById('externalConnection-id')->patch($requestRequestBody);


```