---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/identityProviders/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.Identity().B2cUserFlowsById("b2cIdentityUserFlow-id").IdentityProviders().$ref().Post(requestBody)


```