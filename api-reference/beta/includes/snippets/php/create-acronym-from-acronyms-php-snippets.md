---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Acronym();


$requestRequestBody->setDisplayName('DNN');
$requestRequestBody->setStandsFor('Deep Neural Network');
$requestRequestBody->setDescription('A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers.');
$requestRequestBody->setWebUrl('http://microsoft.com/deep-neural-network');
$requestRequestBody->setState(new AnswerState('draft'));
$result =  $graphClient->search()->acronyms()->post($requestRequestBody);


```