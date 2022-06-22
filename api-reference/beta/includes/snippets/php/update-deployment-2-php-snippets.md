---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Deployment();



$settings = new DeploymentSettings();
$requestRequestBody->setSettings($settings);



$monitoring = new MonitoringSettings();
$settings->setMonitoring($monitoring);


$monitoringRulesArray = [];

$monitoringRules1 = new MonitoringRule();

$monitoringRules1->setSignal(new MonitoringSignal('rollback'));
$monitoringRules1->setThreshold(5);
$monitoringRules1->setAction(new MonitoringAction('pauseDeployment'));

$monitoringRulesArray []= $monitoringRules1;
$monitoring->setMonitoringRules($monitoringRulesArray);

$settingsAdditionalData = [
"@odata.type" => 'microsoft.graph.windowsUpdates.windowsDeploymentSettings',
];
$settings->setAdditionalData($settingsAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.deployment',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->admin()->windows()->updates()->deploymentsById('deployment-id')->patch($requestRequestBody);


```