---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.deployment')

settings = DeploymentSettings()
settings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings')

settingsMonitoring = MonitoringSettings()
monitoringRulesMonitoringRule1 = MonitoringRule()
monitoringRulesMonitoringRule1.setSignal(MonitoringSignal('rollback'))

monitoringRulesMonitoringRule1.setThreshold(5)

monitoringRulesMonitoringRule1.setAction(MonitoringAction('pausedeployment'))


monitoringRulesArray []= monitoringRulesMonitoringRule1;
settingsMonitoring.setMonitoringRules(monitoringRulesArray)



settings.setMonitoring($settingsMonitoring)

request_body.setSettings($settings)


result = await client.admin.windows.updates.deploymentsby_id('deployment-id').patch(request_body)


```