---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AddKeyPostRequestBody();



$keyCredential = new KeyCredential();
$requestRequestBody->setKeyCredential($keyCredential);


$keyCredential->setType('X509CertAndPassword');
$keyCredential->setUsage('Sign');
$keyCredential->setKey(base64_decode("MIIDYDCCAki...")););


$passwordCredential = new PasswordCredential();
$requestRequestBody->setPasswordCredential($passwordCredential);


$passwordCredential->setSecretText('MKTr0w1...');

$requestRequestBody->setProof('eyJ0eXAiOiJ...');
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->addKey()->post($requestRequestBody);


```