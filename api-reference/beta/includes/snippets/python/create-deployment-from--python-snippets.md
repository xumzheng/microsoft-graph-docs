---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.@odatatype = '#microsoft.graph.windowsUpdates.deployment'

content = DeployableContent()
content.@odatatype = '#microsoft.graph.windowsUpdates.catalogContent'

additionalData = [
'catalogEntry' => content = CatalogEntry()
		content.@odatatype = '#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry'

		content.id = 'f341705b-0b15-4ce3-aaf2-6a1681d78606'


content.catalogEntry = catalogEntry

];
content.additionaldata(additionalData)



request_body.content = content
settings = DeploymentSettings()
settings.@odatatype = 'microsoft.graph.windowsUpdates.deploymentSettings'

settingsSchedule = ScheduleSettings()
settingsScheduleGradualRollout = GradualRolloutSettings()
settingsScheduleGradualRollout.@odatatype = '#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings'

settingsScheduleGradualRollout.durationbetweenoffers =  \DateInterval('P7D')

additionalData = [
'devicePerOffer' => 100,
];
settingsScheduleGradualRollout.additionaldata(additionalData)



settingsSchedule.gradualRollout = settingsScheduleGradualRollout

settings.schedule = settingsSchedule
settingsMonitoring = MonitoringSettings()
monitoringRulesMonitoringRule1 = MonitoringRule()
monitoringRulesMonitoringRule1.Signal(MonitoringSignal('rollback'))

monitoringRulesMonitoringRule1.threshold = 5

monitoringRulesMonitoringRule1.Action(MonitoringAction('pausedeployment'))


monitoringRulesArray []= monitoringRulesMonitoringRule1;
settingsMonitoring.monitoringrules(monitoringRulesArray)



settings.monitoring = settingsMonitoring

request_body.settings = settings


request_configuration = DeploymentsRequestBuilderPostRequestConfiguration(
)


result = await client.admin.windows.updates.deployments.post(request_body = request_body)


```