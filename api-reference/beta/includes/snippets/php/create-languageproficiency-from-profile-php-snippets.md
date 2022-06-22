---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LanguageProficiency();


$requestRequestBody->setDisplayName('Norwegian Bokmål');
$requestRequestBody->setTag('nb-NO');
$requestRequestBody->setSpoken(new LanguageProficiencyLevel('nativeOrBilingual'));
$requestRequestBody->setWritten(new LanguageProficiencyLevel('nativeOrBilingual'));
$requestRequestBody->setReading(new LanguageProficiencyLevel('nativeOrBilingual'));
$result =  $graphClient->me()->profile()->languages()->post($requestRequestBody);


```