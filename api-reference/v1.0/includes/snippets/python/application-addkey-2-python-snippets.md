---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AddKeyPostRequestBody();
$keyCredential = new KeyCredential();
$keyCredential.setType('X509CertAndPassword');

$keyCredential.setUsage('Sign');

$KeyCredential.setKey(base64_decode('MIIDYDCCAki...'));


$requestBody.setKeyCredential($keyCredential);
$passwordCredential = new PasswordCredential();
$passwordCredential.setSecretText('MKTr0w1...');


$requestBody.setPasswordCredential($passwordCredential);
$requestBody.setProof('eyJ0eXAiOiJ...');



$requestResult = $graphServiceClient.applicationsById('application-id').addKey().post($requestBody);


```