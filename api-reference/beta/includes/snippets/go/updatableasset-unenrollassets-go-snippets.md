---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewUnenrollAssetsPostRequestBody()
updateCategory := graphmodels.STRING_UPDATECATEGORY 
requestBody.SetUpdateCategory(&updateCategory) 


updatableAsset := graphmodels.NewUpdatableAsset()
additionalData := map[string]interface{}{
	"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice", 
	"id" : "String (identifier)", 
}
updatableAsset.SetAdditionalData(additionalData)

assets := []graphmodels.UpdatableAssetable {
	updatableAsset,

}
requestBody.SetAssets(assets)

graphClient.Admin().Windows().Updates().UpdatableAssets().UnenrollAssets().Post(requestBody)


```