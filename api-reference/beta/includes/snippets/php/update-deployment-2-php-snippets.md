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

$monitoringRulesmonitoringRules1 = new MonitoringRule();

$monitoringRulesmonitoringRules1->setSignal(new MonitoringSignal('rollback'));
$monitoringRulesmonitoringRules1->setThreshold(5);
$monitoringRulesmonitoringRules1->setAction(new MonitoringAction('pauseDeployment'));

$monitoringRulesArray []= $monitoringRulesmonitoringRules1;
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