---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UpdatePolicy();
request_body.set@odatatype('#microsoft.graph.windowsUpdates.updatePolicy');

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

request_body.setDeploymentSettings($deploymentSettings);


result = await client.admin.windows.updates.updatePoliciesById('updatePolicy-id').patch(request_body);


```