---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.New$refPostRequestBody()
additionalData := map[string]interface{}{
	"@odata.id" : "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.OnPremisesPublishingProfilesById("onPremisesPublishingProfile-id").ConnectorGroupsById("connectorGroup-id").Members().$ref().Post(requestBody)


```