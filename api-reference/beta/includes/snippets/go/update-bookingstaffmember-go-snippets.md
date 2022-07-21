---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewBookingStaffMember()


bookingWorkHours := graphmodels.NewBookingWorkHours()
odataType := "#microsoft.graph.bookingWorkHours"
bookingWorkHours.SetOdataType(&odataType) 
day := graphmodels.MONDAY_DAYOFWEEK 
bookingWorkHours.SetDay(&day) 
timeSlots := []graphmodels.BookingWorkTimeSlotable {

}
bookingWorkHours.SetTimeSlots(timeSlots)
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.dayOfWeek", 
	"odataType" : "#Collection(microsoft.graph.bookingWorkTimeSlot)", 
}
bookingWorkHours.SetAdditionalData(additionalData)
bookingWorkHours1 := graphmodels.NewBookingWorkHours()
odataType := "#microsoft.graph.bookingWorkHours"
bookingWorkHours1.SetOdataType(&odataType) 
day := graphmodels.TUESDAY_DAYOFWEEK 
bookingWorkHours1.SetDay(&day) 


bookingWorkTimeSlot := graphmodels.NewBookingWorkTimeSlot()
odataType := "#microsoft.graph.bookingWorkTimeSlot"
bookingWorkTimeSlot.SetOdataType(&odataType) 
end := "17:00:00.0000000"
bookingWorkTimeSlot.SetEnd(&end) 
start := "08:00:00.0000000"
bookingWorkTimeSlot.SetStart(&start) 

timeSlots := []graphmodels.BookingWorkTimeSlotable {
	bookingWorkTimeSlot,

}
bookingWorkHours1.SetTimeSlots(timeSlots)
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.dayOfWeek", 
	"odataType" : "#Collection(microsoft.graph.bookingWorkTimeSlot)", 
}
bookingWorkHours1.SetAdditionalData(additionalData)
bookingWorkHours2 := graphmodels.NewBookingWorkHours()
odataType := "#microsoft.graph.bookingWorkHours"
bookingWorkHours2.SetOdataType(&odataType) 
day := graphmodels.WEDNESDAY_DAYOFWEEK 
bookingWorkHours2.SetDay(&day) 


bookingWorkTimeSlot := graphmodels.NewBookingWorkTimeSlot()
odataType := "#microsoft.graph.bookingWorkTimeSlot"
bookingWorkTimeSlot.SetOdataType(&odataType) 
end := "17:00:00.0000000"
bookingWorkTimeSlot.SetEnd(&end) 
start := "08:00:00.0000000"
bookingWorkTimeSlot.SetStart(&start) 

timeSlots := []graphmodels.BookingWorkTimeSlotable {
	bookingWorkTimeSlot,

}
bookingWorkHours2.SetTimeSlots(timeSlots)
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.dayOfWeek", 
	"odataType" : "#Collection(microsoft.graph.bookingWorkTimeSlot)", 
}
bookingWorkHours2.SetAdditionalData(additionalData)
bookingWorkHours3 := graphmodels.NewBookingWorkHours()
odataType := "#microsoft.graph.bookingWorkHours"
bookingWorkHours3.SetOdataType(&odataType) 
day := graphmodels.THURSDAY_DAYOFWEEK 
bookingWorkHours3.SetDay(&day) 


bookingWorkTimeSlot := graphmodels.NewBookingWorkTimeSlot()
odataType := "#microsoft.graph.bookingWorkTimeSlot"
bookingWorkTimeSlot.SetOdataType(&odataType) 
end := "17:00:00.0000000"
bookingWorkTimeSlot.SetEnd(&end) 
start := "08:00:00.0000000"
bookingWorkTimeSlot.SetStart(&start) 

timeSlots := []graphmodels.BookingWorkTimeSlotable {
	bookingWorkTimeSlot,

}
bookingWorkHours3.SetTimeSlots(timeSlots)
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.dayOfWeek", 
	"odataType" : "#Collection(microsoft.graph.bookingWorkTimeSlot)", 
}
bookingWorkHours3.SetAdditionalData(additionalData)
bookingWorkHours4 := graphmodels.NewBookingWorkHours()
odataType := "#microsoft.graph.bookingWorkHours"
bookingWorkHours4.SetOdataType(&odataType) 
day := graphmodels.FRIDAY_DAYOFWEEK 
bookingWorkHours4.SetDay(&day) 


bookingWorkTimeSlot := graphmodels.NewBookingWorkTimeSlot()
odataType := "#microsoft.graph.bookingWorkTimeSlot"
bookingWorkTimeSlot.SetOdataType(&odataType) 
end := "17:00:00.0000000"
bookingWorkTimeSlot.SetEnd(&end) 
start := "08:00:00.0000000"
bookingWorkTimeSlot.SetStart(&start) 

timeSlots := []graphmodels.BookingWorkTimeSlotable {
	bookingWorkTimeSlot,

}
bookingWorkHours4.SetTimeSlots(timeSlots)
additionalData := map[string]interface{}{
	"odataType" : "#microsoft.graph.dayOfWeek", 
	"odataType" : "#Collection(microsoft.graph.bookingWorkTimeSlot)", 
}
bookingWorkHours4.SetAdditionalData(additionalData)

workingHours := []graphmodels.BookingWorkHoursable {
	bookingWorkHours,
	bookingWorkHours1,
	bookingWorkHours2,
	bookingWorkHours3,
	bookingWorkHours4,

}
requestBody.SetWorkingHours(workingHours)

graphClient.BookingBusinessesById("bookingBusiness-id").StaffMembersById("bookingStaffMember-id").Patch(requestBody)


```