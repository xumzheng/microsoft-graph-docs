---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewUpdateAudiencePostRequestBody()


updatableAsset := graphmodels.NewUpdatableAsset()
additionalData := map[string]interface{}{
	"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice", 
	"id" : "String (identifier)", 
}
updatableAsset.SetAdditionalData(additionalData)

addMembers := []graphmodels.UpdatableAssetable {
	updatableAsset,

}
requestBody.SetAddMembers(addMembers)


updatableAsset := graphmodels.NewUpdatableAsset()
additionalData := map[string]interface{}{
	"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice", 
	"id" : "String (identifier)", 
}
updatableAsset.SetAdditionalData(additionalData)

removeMembers := []graphmodels.UpdatableAssetable {
	updatableAsset,

}
requestBody.SetRemoveMembers(removeMembers)


updatableAsset := graphmodels.NewUpdatableAsset()
additionalData := map[string]interface{}{
	"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice", 
	"id" : "String (identifier)", 
}
updatableAsset.SetAdditionalData(additionalData)

addExclusions := []graphmodels.UpdatableAssetable {
	updatableAsset,

}
requestBody.SetAddExclusions(addExclusions)


updatableAsset := graphmodels.NewUpdatableAsset()
additionalData := map[string]interface{}{
	"@odata.type" : "#microsoft.graph.windowsUpdates.azureADDevice", 
	"id" : "String (identifier)", 
}
updatableAsset.SetAdditionalData(additionalData)

removeExclusions := []graphmodels.UpdatableAssetable {
	updatableAsset,

}
requestBody.SetRemoveExclusions(removeExclusions)

graphClient.Admin().Windows().Updates().DeploymentsById("deployment-id").Audience().UpdateAudience(deployment-id).Post(requestBody)


```