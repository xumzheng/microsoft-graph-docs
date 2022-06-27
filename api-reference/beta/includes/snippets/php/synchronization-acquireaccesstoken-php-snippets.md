---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CredentialsRequestBody();


$credentialsArray = [];

$credentialscredentials1 = new SynchronizationSecretKeyStringValuePair();

$credentialscredentials1AdditionalData = [
	"@odata.type" => 'microsoft.graph.synchronizationSecretKeyStringValuePair',
];
$credentialscredentials1->setAdditionalData($credentialscredentials1AdditionalData);

$credentialsArray []= $credentialscredentials1;
$requestRequestBody->setCredentials($credentialsArray);
$result =  $graphClient->applicationsById('application-id')->synchronization()->acquireAccessToken()->post($requestRequestBody);


```