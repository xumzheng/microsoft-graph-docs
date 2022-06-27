---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InferenceClassificationOverride();


$requestRequestBody->setClassifyAs(new InferenceClassificationType('focused'));

$senderEmailAddress = new EmailAddress();
$requestRequestBody->setSenderEmailAddress($senderEmailAddress);


$senderEmailAddress->setName('Samantha Booth');
$senderEmailAddress->setAddress('samanthab@adatum.onmicrosoft.com');

$result =  $graphClient->me()->inferenceClassification()->overrides()->post($requestRequestBody);


```