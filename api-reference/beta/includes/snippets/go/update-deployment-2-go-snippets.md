---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewDeployment()
odataType := "#microsoft.graph.windowsUpdates.deployment"
requestBody.SetOdataType(&odataType) 
settings := graphmodels.NewDeploymentSettings()
odataType := "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
settings.SetOdataType(&odataType) 
monitoring := graphmodels.NewMonitoringSettings()


monitoringRule := graphmodels.NewMonitoringRule()
signal := graphmodels.ROLLBACK_MONITORINGSIGNAL 
monitoringRule.SetSignal(&signal) 
threshold := int32(5)
monitoringRule.SetThreshold(&threshold) 
action := graphmodels.PAUSEDEPLOYMENT_MONITORINGACTION 
monitoringRule.SetAction(&action) 

monitoringRules := []graphmodels.MonitoringRuleable {
	monitoringRule,

}
monitoring.SetMonitoringRules(monitoringRules)
settings.SetMonitoring(monitoring)
requestBody.SetSettings(settings)

graphClient.Admin().Windows().Updates().DeploymentsById("deployment-id").Patch(requestBody)


```