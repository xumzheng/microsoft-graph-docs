---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Deployment();



$content = new DeployableContent();
$requestRequestBody->setContent($content);


$contentAdditionalData = [
	"@odata.type" => 'microsoft.graph.windowsUpdates.featureUpdateReference',
	"version" => '20H2',
];
$content->setAdditionalData($contentAdditionalData);


$settings = new DeploymentSettings();
$requestRequestBody->setSettings($settings);



$rollout = new RolloutSettings();
$settings->setRollout($rollout);


$rollout->setDevicesPerOffer(100);


$monitoring = new MonitoringSettings();
$settings->setMonitoring($monitoring);


$monitoringRulesArray = [];

$monitoringRules1 = new MonitoringRule();

$monitoringRules1->setSignal(new MonitoringSignal('rollback'));
$monitoringRules1->setThreshold(5);
$monitoringRules1->setAction(new MonitoringAction('pauseDeployment'));
$monitoringRules1AdditionalData = [
"@odata.type" => '#microsoft.graph.windowsUpdates.monitoringRule',
];
$monitoringRules1->setAdditionalData($monitoringRules1AdditionalData);

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
$result =  $graphClient->admin()->windows()->updates()->deployments()->post($requestRequestBody);


```