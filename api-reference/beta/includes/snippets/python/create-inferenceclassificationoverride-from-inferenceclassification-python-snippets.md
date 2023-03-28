---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InferenceClassificationOverride();
$requestBody->setClassifyAs(new InferenceClassificationType('focused'));

$senderEmailAddress = new EmailAddress();
$senderEmailAddress->setName('Samantha Booth');

$senderEmailAddress->setAddress('samanthab@adatum.onmicrosoft.com');


$requestBody->setSenderEmailAddress($senderEmailAddress);


$requestResult = $graphServiceClient->me()->inferenceClassification()->overrides()->post($requestBody);


```