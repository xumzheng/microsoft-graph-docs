---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.New$refPostRequestBody()
additionalData := map[string]interface{}{
	"@odata.id" : "https://graph.microsoft.com/beta/identityProviders/{id}", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Identity().B2cUserFlowsById("b2cIdentityUserFlow-id").IdentityProviders().$ref().Post(requestBody)


```