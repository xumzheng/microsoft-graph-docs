---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDescription('Self help community for golf');
$requestRequestBody->setDisplayName('Golf Assist');
$requestRequestBody->setGroupTypes( [
'Unified',],
$requestRequestBody->setMailEnabled(True);
$requestRequestBody->setMailNickname('golfassist');
$requestRequestBody->setSecurityEnabled(False);
$result =  $graphClient->groups()->post($requestRequestBody);


```