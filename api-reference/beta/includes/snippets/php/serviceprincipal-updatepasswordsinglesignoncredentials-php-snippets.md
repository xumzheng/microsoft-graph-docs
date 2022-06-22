---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdatePasswordSingleSignOnCredentialsPostRequestBody();


$requestRequestBody->setId('5793aa3b-cca9-4794-679a240f8b58');
$credentialsArray = [];

$credentials1 = new Credential();

$credentials1AdditionalData = [
		"fieldId" => 'param_username',
		"value" => 'myusername',
		"type" => 'username',
	];
$credentials1->setAdditionalData($credentials1AdditionalData);

$credentialsArray []= $credentials1;

$credentials2 = new Credential();

$credentials2AdditionalData = [
	"fieldId" => 'param_password',
	"value" => 'pa$$w0rd',
	"type" => 'password',
];
$credentials2->setAdditionalData($credentials2AdditionalData);

$credentialsArray []= $credentials2;
$requestRequestBody->setCredentials($credentialsArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->updatePasswordSingleSignOnCredentials()->post($requestRequestBody);


```