---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CredentialsRequestBody();


$credentialsArray = [];

$credentials1 = new SynchronizationSecretKeyStringValuePair();

$credentials1AdditionalData = [
		"@odata.type" => 'microsoft.graph.synchronizationSecretKeyStringValuePair',
	];
$credentials1->setAdditionalData($credentials1AdditionalData);

$credentialsArray []= $credentials1;
$requestRequestBody->setCredentials($credentialsArray);
$result =  $graphClient->applicationsById('application-id')->synchronization()->acquireAccessToken()->post($requestRequestBody);


```