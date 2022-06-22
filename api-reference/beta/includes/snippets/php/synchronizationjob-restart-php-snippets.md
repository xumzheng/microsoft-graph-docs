---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CriteriaRequestBody();



$criteria = new SynchronizationJobRestartCriteria();
$requestRequestBody->setCriteria($criteria);


$criteria->setResetScope(new SynchronizationJobRestartScope('Watermark, Escrows, QuarantineState'));

$requestConfiguration = new RestartRequestBuilderPostRequestConfiguration();

$headers = [
"Authorization" => "Bearer <token>",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->restart()->post($requestRequestBody, $requestConfiguration);


```