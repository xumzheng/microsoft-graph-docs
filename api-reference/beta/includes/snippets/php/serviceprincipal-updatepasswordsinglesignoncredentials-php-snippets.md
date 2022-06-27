---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdatePasswordSingleSignOnCredentialsPostRequestBody();


$requestRequestBody->setId('5793aa3b-cca9-4794-679a240f8b58');
$credentialsArray = [];

$credentialscredentials1 = new Credential();

$credentialscredentials1AdditionalData = [
	"fieldId" => 'param_username',
	"value" => 'myusername',
	"type" => 'username',
];
$credentialscredentials1->setAdditionalData($credentialscredentials1AdditionalData);

$credentialsArray []= $credentialscredentials1;

$credentialscredentials2 = new Credential();

$credentialscredentials2AdditionalData = [
"fieldId" => 'param_password',
"value" => 'pa$$w0rd',
"type" => 'password',
];
$credentialscredentials2->setAdditionalData($credentialscredentials2AdditionalData);

$credentialsArray []= $credentialscredentials2;
$requestRequestBody->setCredentials($credentialsArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->updatePasswordSingleSignOnCredentials()->post($requestRequestBody);


```