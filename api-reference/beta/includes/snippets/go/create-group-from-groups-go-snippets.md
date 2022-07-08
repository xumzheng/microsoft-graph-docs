---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.New$refPostRequestBody()
additionalData := map[string]interface{}{
	"@odata.id" : "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Policies().MobileAppManagementPoliciesById("mobilityManagementPolicy-id").IncludedGroups().$ref().Post(requestBody)


```