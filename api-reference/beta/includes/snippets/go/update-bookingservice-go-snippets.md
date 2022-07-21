---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewBookingService()
odataType := "#microsoft.graph.bookingService"
requestBody.SetOdataType(&odataType) 
defaultDuration := "PT30M"
requestBody.SetDefaultDuration(&defaultDuration) 

graphClient.BookingBusinessesById("bookingBusiness-id").ServicesById("bookingService-id").Patch(requestBody)


```