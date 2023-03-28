---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UpdatePolicy();
$requestBody.set@odatatype('#microsoft.graph.windowsUpdates.updatePolicy');

$deploymentSettings = new DeploymentSettings();
$deploymentSettings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings');

$deploymentSettingsSchedule = new ScheduleSettings();
$deploymentSettingsScheduleGradualRollout = new GradualRolloutSettings();
$deploymentSettingsScheduleGradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings');

$deploymentSettingsScheduleGradualRollout.setDurationBetweenOffers(new \DateInterval('P1D'));

$additionalData = [
'devicePerOffer' => 1000,
];
$deploymentSettingsScheduleGradualRollout.setAdditionalData($additionalData);



$deploymentSettingsSchedule.setGradualRollout($deploymentSettingsScheduleGradualRollout);

$deploymentSettings.setSchedule($deploymentSettingsSchedule);

$requestBody.setDeploymentSettings($deploymentSettings);


$requestResult = $graphServiceClient.admin().windows().updates().updatePoliciesById('updatePolicy-id').patch($requestBody);


```