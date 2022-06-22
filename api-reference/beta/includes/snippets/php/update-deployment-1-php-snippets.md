---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Deployment();



$state = new DeploymentState();
$requestRequestBody->setState($state);


$state->setRequestedValue(new RequestedDeploymentStateValue('paused'));
$stateAdditionalData = [
	"@odata.type" => 'microsoft.graph.windowsUpdates.deploymentState',
];
$state->setAdditionalData($stateAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.deployment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->admin()->windows()->updates()->deploymentsById('deployment-id')->patch($requestRequestBody);


```