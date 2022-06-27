---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TrustFrameworkKeySet();


$requestRequestBody->setId('keyset1');
$keysArray = [];

$keyskeys1 = new TrustFrameworkKey();

$keyskeys1->setK('k-value');
$keyskeys1->setX5c(['x5c-value',]);
$keyskeys1->setX5t('x5t-value');
$keyskeys1->setKty('kty-value');
$keyskeys1->setUse('use-value');
$keyskeys1->setExp(99);
$keyskeys1->setNbf(99);
$keyskeys1->setKid('kid-value');
$keyskeys1->setE('e-value');
$keyskeys1->setN('n-value');
$keyskeys1->setD('d-value');
$keyskeys1->setP('p-value');
$keyskeys1->setQ('q-value');
$keyskeys1->setDp('dp-value');
$keyskeys1->setDq('dq-value');
$keyskeys1->setQi('qi-value');

$keysArray []= $keyskeys1;
$requestRequestBody->setKeys($keysArray);
$result =  $graphClient->trustFramework()->keySets()->post($requestRequestBody);


```