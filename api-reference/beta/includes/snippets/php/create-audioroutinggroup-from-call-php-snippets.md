---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AudioRoutingGroup();


$requestRequestBody->setId('oneToOne');
$requestRequestBody->setRoutingMode(new RoutingMode('oneToOne'));
$requestRequestBody->setSources( [
'632899f8-2ea1-4604-8413-27bd2892079f',],
$requestRequestBody->setReceivers( [
'550fae72-d251-43ec-868c-373732c2704f',],
$result =  $graphClient->communications()->callsById('call-id')->audioRoutingGroups()->post($requestRequestBody);


```