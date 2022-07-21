---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewUpdatableAsset()
odataType := "#microsoft.graph.windowsUpdates.updatableAssetGroup"
requestBody.SetOdataType(&odataType) 

result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Post(requestBody)


```