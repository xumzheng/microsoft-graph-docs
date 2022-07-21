---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewBookingAppointment()
odataType := "#microsoft.graph.bookingAppointment"
requestBody.SetOdataType(&odataType) 
endDateTime := graphmodels.NewDateTimeTimeZone()
odataType := "#microsoft.graph.dateTimeTimeZone"
endDateTime.SetOdataType(&odataType) 
dateTime := "2018-05-06T12:30:00.0000000+00:00"
endDateTime.SetDateTime(&dateTime) 
timeZone := "UTC"
endDateTime.SetTimeZone(&timeZone) 
requestBody.SetEndDateTime(endDateTime)
startDateTime := graphmodels.NewDateTimeTimeZone()
odataType := "#microsoft.graph.dateTimeTimeZone"
startDateTime.SetOdataType(&odataType) 
dateTime := "2018-05-06T12:00:00.0000000+00:00"
startDateTime.SetDateTime(&dateTime) 
timeZone := "UTC"
startDateTime.SetTimeZone(&timeZone) 
requestBody.SetStartDateTime(startDateTime)

graphClient.Solutions().BookingBusinessesById("bookingBusiness-id").AppointmentsById("bookingAppointment-id").Patch(requestBody)


```