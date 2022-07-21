---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewPlannerRoster()
odataType := "#microsoft.graph.plannerRoster"
requestBody.SetOdataType(&odataType) 

result, err := graphClient.Planner().Rosters().Post(requestBody)


```