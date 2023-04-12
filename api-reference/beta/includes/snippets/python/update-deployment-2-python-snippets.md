---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.deployment'

settings = DeploymentSettings()
settings.@odatatype = 'microsoft.graph.windowsUpdates.deploymentSettings'

settingsMonitoring = MonitoringSettings()
monitoringRulesMonitoringRule1 = MonitoringRule()
monitoringRulesMonitoringRule1.Signal(MonitoringSignal('rollback'))

monitoringRulesMonitoringRule1.threshold = 5

monitoringRulesMonitoringRule1.Action(MonitoringAction('pausedeployment'))


monitoringRulesArray []= monitoringRulesMonitoringRule1;
settingsMonitoring.monitoringrules(monitoringRulesArray)



settings.monitoring = settingsMonitoring

request_body.settings = settings



result = await client.admin.windows.updates.deployments_by_id('deployment-id').patch(request_body = request_body)


```