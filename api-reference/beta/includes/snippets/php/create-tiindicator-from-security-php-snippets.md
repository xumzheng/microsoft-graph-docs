---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TiIndicator();


$requestRequestBody->setAction(new TiAction('alert'));
$requestRequestBody->setActivityGroupNames([]);
$requestRequestBody->setConfidence(0);
$requestRequestBody->setDescription('This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.');
$requestRequestBody->setExpirationDateTime(new DateTime("2019-03-01T21:43:37.5031462+00:00"));
$requestRequestBody->setExternalId('Test--8586509942679764298MS501');
$requestRequestBody->setFileHashType(new FileHashType('sha256'));
$requestRequestBody->setFileHashValue('aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313');
$requestRequestBody->setKillChain([]);
$requestRequestBody->setMalwareFamilyNames([]);
$requestRequestBody->setSeverity(0);
$requestRequestBody->setTags([]);
$requestRequestBody->setTargetProduct('Azure Sentinel');
$requestRequestBody->setThreatType('WatchList');
$requestRequestBody->setTlpLevel(new TlpLevel('green'));
$result =  $graphClient->security()->tiIndicators()->post($requestRequestBody);


```