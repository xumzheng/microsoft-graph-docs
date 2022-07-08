---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewUpdateTiIndicatorsPostRequestBody()


tiIndicator := graphmodels.NewTiIndicator()
additionalData := map[string]interface{}{
	"id" : "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4", 
	"additionalInformation" : "mytest", 
}
tiIndicator.SetAdditionalData(additionalData)
tiIndicator1 := graphmodels.NewTiIndicator()
additionalData := map[string]interface{}{
	"id" : "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e", 
	"additionalInformation" : "test again", 
}
tiIndicator1.SetAdditionalData(additionalData)

value := []graphmodels.TiIndicatorable {
	tiIndicator,
	tiIndicator1,

}
requestBody.SetValue(value)

result, err := graphClient.Security().TiIndicators().UpdateTiIndicators().Post(requestBody)


```