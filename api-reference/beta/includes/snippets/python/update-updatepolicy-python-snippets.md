---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UpdatePolicy();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.updatePolicy');

deploymentSettings = DeploymentSettings();
deploymentSettings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings');

deploymentSettingsSchedule = ScheduleSettings();
deploymentSettingsScheduleGradualRollout = GradualRolloutSettings();
deploymentSettingsScheduleGradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings');

$deploymentSettingsScheduleGradualRollout.setDurationBetweenOffers( \DateInterval('P1D'));

additionalData = [
'devicePerOffer' => 1000,
];
deploymentSettingsScheduleGradualRollout.setAdditionalData(additionalData);



deploymentSettingsSchedule.setGradualRollout($deploymentSettingsScheduleGradualRollout);

deploymentSettings.setSchedule($deploymentSettingsSchedule);

requestBody.setDeploymentSettings($deploymentSettings);


requestResult = graphServiceClient.admin().windows().updates().updatePoliciesById('updatePolicy-id').patch(requestBody);


```