---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewIdentityProviderBase()
odataType := "#microsoft.graph.socialIdentityProvider"
requestBody.SetOdataType(&odataType) 
additionalData := map[string]interface{}{
	"clientSecret" : "1111111111111", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().IdentityProvidersById("identityProviderBase-id").Patch(requestBody)


```