---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewPrinterShare()
name := "name-value"
requestBody.SetName(&name) 
additionalData := map[string]interface{}{
	"odataBind" : "https://graph.microsoft.com/beta/print/printers/{id}", 
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Print().Shares().Post(requestBody)


```