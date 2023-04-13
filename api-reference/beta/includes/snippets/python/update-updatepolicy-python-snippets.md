---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdatePolicy()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.updatePolicy'

deployment_settings = DeploymentSettings()
deploymentSettings.@odatatype = 'microsoft.graph.windowsUpdates.deploymentSettings'

deployment_settings_schedule = ScheduleSettings()
deployment_settings_schedule_gradual_rollout = GradualRolloutSettings()
deploymentSettingsScheduleGradualRollout.@odatatype = '#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings'

deploymentSettingsScheduleGradualRollout.durationbetweenoffers =  \DateInterval('P1D')

additionalData = [
'devicePerOffer' => 1000,
];
deploymentSettingsScheduleGradualRollout.additionaldata(additionalData)



deploymentSettingsSchedule.gradual_rollout = deploymentSettingsScheduleGradualRollout

deploymentSettings.schedule = deploymentSettingsSchedule

request_body.deployment_settings = deploymentSettings



result = await client.admin.windows.updates.updatePolicies_by_id('updatePolicy-id').patch(request_body = request_body)


```