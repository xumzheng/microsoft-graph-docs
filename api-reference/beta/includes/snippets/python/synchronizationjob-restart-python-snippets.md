---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RestartPostRequestBody();
$criteria = new SynchronizationJobRestartCriteria();
$criteria->setResetScope(new SynchronizationJobRestartScope('watermark, escrows, quarantinestate'));


$requestBody->setCriteria($criteria);

$requestConfiguration = new RestartRequestBuilderPostRequestConfiguration();

$headers = [
	'Authorization' => 'Bearer <token>',
];

$requestConfiguration->headers = $headers;


$graphServiceClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->restart()->post($requestBody, $requestConfiguration);


```