---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdatePolicy()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.updatePolicy'

deploymentSettings = DeploymentSettings()
deploymentSettings.@odatatype = 'microsoft.graph.windowsUpdates.deploymentSettings'

deploymentSettingsSchedule = ScheduleSettings()
deploymentSettingsScheduleGradualRollout = GradualRolloutSettings()
deploymentSettingsScheduleGradualRollout.@odatatype = '#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings'

deploymentSettingsScheduleGradualRollout.durationbetweenoffers =  \DateInterval('P1D')

additionalData = [
'devicePerOffer' => 1000,
];
deploymentSettingsScheduleGradualRollout.additionaldata(additionalData)



deploymentSettingsSchedule.gradualRollout = deploymentSettingsScheduleGradualRollout

deploymentSettings.schedule = deploymentSettingsSchedule

request_body.deploymentSettings = deploymentSettings


request_configuration = UpdatePolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.admin.windows.updates.updatePolicies_by_id('updatePolicy-id').patch(request_body = request_body)


```