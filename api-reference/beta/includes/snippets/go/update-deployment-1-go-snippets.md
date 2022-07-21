---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewDeployment()
odataType := "#microsoft.graph.windowsUpdates.deployment"
requestBody.SetOdataType(&odataType) 
state := graphmodels.NewDeploymentState()
odataType := "microsoft.graph.windowsUpdates.deploymentState"
state.SetOdataType(&odataType) 
requestedValue := graphmodels.PAUSED_REQUESTEDDEPLOYMENTSTATEVALUE 
state.SetRequestedValue(&requestedValue) 
requestBody.SetState(state)

graphClient.Admin().Windows().Updates().DeploymentsById("deployment-id").Patch(requestBody)


```