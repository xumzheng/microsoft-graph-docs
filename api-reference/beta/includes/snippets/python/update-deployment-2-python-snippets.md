---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Deployment();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.deployment');

settings = DeploymentSettings();
settings.set@odatatype('microsoft.graph.windowsUpdates.deploymentSettings');

settingsMonitoring = MonitoringSettings();
monitoringRulesMonitoringRule1 = MonitoringRule();
monitoringRulesMonitoringRule1.setSignal(MonitoringSignal('rollback'));

monitoringRulesMonitoringRule1.setThreshold(5);

monitoringRulesMonitoringRule1.setAction(MonitoringAction('pausedeployment'));


monitoringRulesArray []= monitoringRulesMonitoringRule1;
settingsMonitoring.setMonitoringRules(monitoringRulesArray);



settings.setMonitoring($settingsMonitoring);

requestBody.setSettings($settings);


requestResult = graphServiceClient.admin().windows().updates().deploymentsById('deployment-id').patch(requestBody);


```