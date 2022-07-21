---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewAttachment()
odataType := "#Microsoft.OutlookServices.ItemAttachment"
requestBody.SetOdataType(&odataType) 
name := "name-value"
requestBody.SetName(&name) 
additionalData := map[string]interface{}{
item := graphmodels.New()
odataType := "microsoft.graph.message"
item.SetOdataType(&odataType) 
	requestBody.SetItem(item)
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Me().EventsById("event-id").Attachments().Post(requestBody)


```