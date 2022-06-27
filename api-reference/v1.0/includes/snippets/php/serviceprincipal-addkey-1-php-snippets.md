---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AddKeyPostRequestBody();



$keyCredential = new KeyCredential();
$requestRequestBody->setKeyCredential($keyCredential);


$keyCredential->setType('AsymmetricX509Cert');
$keyCredential->setUsage('Verify');
$keyCredential->setKey(base64_decode("MIIDYDCCAki...")););

$requestRequestBody->setPasswordCredential(null);
$requestRequestBody->setProof('eyJ0eXAiOiJ...');
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->addKey()->post($requestRequestBody);


```