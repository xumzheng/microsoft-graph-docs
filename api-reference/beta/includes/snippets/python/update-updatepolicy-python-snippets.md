---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Update_policy()
request_body.@odata_type = '#microsoft.graph.windowsUpdates.updatePolicy'

deployment_settings = Deployment_settings()
deployment_settings.@odata_type = 'microsoft.graph.windowsUpdates.deploymentSettings'

deployment_settingsschedule = Schedule_settings()
deployment_settingsschedulegradual_rollout = Gradual_rollout_settings()
deployment_settingsschedulegradual_rollout.@odata_type = '#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings'

deployment_settingsschedulegradual_rollout.durationbetweenoffers =  \DateInterval('P1D')

additional_data = [
'device_per_offer' => 1000,
];
deployment_settingsschedulegradual_rollout.additional_data(additional_data)



deployment_settingsschedule.gradual_rollout = deployment_settingsschedulegradual_rollout

deployment_settings.schedule = deployment_settingsschedule

request_body.deployment_settings = deployment_settings



result = await client.admin.windows.updates.update_policies.by_update_policie_id('updatePolicy-id').patch(request_body = request_body)


```