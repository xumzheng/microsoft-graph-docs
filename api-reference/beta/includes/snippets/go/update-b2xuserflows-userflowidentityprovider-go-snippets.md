---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.New$refPostRequestBody()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test", 
	"odataType" : "#microsoft.graph.identityProvider", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Identity().B2xUserFlowsById("b2xIdentityUserFlow-id").UserFlowIdentityProviders().$ref().Patch(requestBody)


```