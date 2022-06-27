---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Acronym();


$requestRequestBody->setDescription('A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.');
$result =  $graphClient->search()->acronymsById('acronym-id')->patch($requestRequestBody);


```