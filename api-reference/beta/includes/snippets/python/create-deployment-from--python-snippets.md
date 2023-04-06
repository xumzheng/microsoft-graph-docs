---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Deployment()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.deployment')

content = DeployableContent()
content.set@odatatype('#microsoft.graph.windowsUpdates.catalogContent')

additionalData = [
'catalogEntry' => content = CatalogEntry()
		content.set@odatatype('#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry')

		content.setId('f341705b-0b15-4ce3-aaf2-6a1681d78606')


content.setCatalogEntry($catalogEntry)

];
content.setAdditionalData(additionalData)



request_body.setContent($content)
settings = DeploymentSettings()
settings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings')

settingsSchedule = ScheduleSettings()
settingsScheduleGradualRollout = GradualRolloutSettings()
settingsScheduleGradualRollout.set@odatatype('#microsoft.graph.windowsUpdates.rateDrivenRolloutSettings')

$settingsScheduleGradualRollout.setDurationBetweenOffers( \DateInterval('P7D'))

additionalData = [
'devicePerOffer' => 100,
];
settingsScheduleGradualRollout.setAdditionalData(additionalData)



settingsSchedule.setGradualRollout($settingsScheduleGradualRollout)

settings.setSchedule($settingsSchedule)
settingsMonitoring = MonitoringSettings()
monitoringRulesMonitoringRule1 = MonitoringRule()
monitoringRulesMonitoringRule1.setSignal(MonitoringSignal('rollback'))

monitoringRulesMonitoringRule1.setThreshold(5)

monitoringRulesMonitoringRule1.setAction(MonitoringAction('pausedeployment'))


monitoringRulesArray []= monitoringRulesMonitoringRule1;
settingsMonitoring.setMonitoringRules(monitoringRulesArray)



settings.setMonitoring($settingsMonitoring)

request_body.setSettings($settings)


result = await client.admin.windows.updates.deployments.post(request_body, headers=)


```