---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingStaffMemberBase()
request_body.set@odatatype('#microsoft.graph.bookingStaffMember')

additionalData = [
'workingHours' => workingHours1 = ()
		workingHours1.set@odatatype('#microsoft.graph.bookingWorkHours')

		workingHours1.setDay@odatatype('#microsoft.graph.dayOfWeek')

		workingHours1.setDay('monday')

		workingHours1.setTimeSlots@odatatype('#Collection(microsoft.graph.bookingWorkTimeSlot)')

workingHours1.setTimeSlots([])


workingHoursArray []= workingHours1;
workingHours2 = ()
	workingHours2.set@odatatype('#microsoft.graph.bookingWorkHours')

	workingHours2.setDay@odatatype('#microsoft.graph.dayOfWeek')

	workingHours2.setDay('tuesday')

	workingHours2.setTimeSlots@odatatype('#Collection(microsoft.graph.bookingWorkTimeSlot)')

timeSlots1 = ()
	timeSlots1.set@odatatype('#microsoft.graph.bookingWorkTimeSlot')

	timeSlots1.setEndTime('17:00:00.0000000')

	timeSlots1.setStartTime('08:00:00.0000000')


timeSlotsArray []= timeSlots1;
workingHours2.setTimeSlots(timeSlotsArray)



workingHoursArray []= workingHours2;
workingHours3 = ()
workingHours3.set@odatatype('#microsoft.graph.bookingWorkHours')

workingHours3.setDay@odatatype('#microsoft.graph.dayOfWeek')

workingHours3.setDay('wednesday')

workingHours3.setTimeSlots@odatatype('#Collection(microsoft.graph.bookingWorkTimeSlot)')

timeSlots1 = ()
timeSlots1.set@odatatype('#microsoft.graph.bookingWorkTimeSlot')

timeSlots1.setEndTime('17:00:00.0000000')

timeSlots1.setStartTime('08:00:00.0000000')


timeSlotsArray []= timeSlots1;
workingHours3.setTimeSlots(timeSlotsArray)



workingHoursArray []= workingHours3;
workingHours4 = ()
workingHours4.set@odatatype('#microsoft.graph.bookingWorkHours')

workingHours4.setDay@odatatype('#microsoft.graph.dayOfWeek')

workingHours4.setDay('thursday')

workingHours4.setTimeSlots@odatatype('#Collection(microsoft.graph.bookingWorkTimeSlot)')

timeSlots1 = ()
timeSlots1.set@odatatype('#microsoft.graph.bookingWorkTimeSlot')

timeSlots1.setEndTime('17:00:00.0000000')

timeSlots1.setStartTime('08:00:00.0000000')


timeSlotsArray []= timeSlots1;
workingHours4.setTimeSlots(timeSlotsArray)



workingHoursArray []= workingHours4;
workingHours5 = ()
workingHours5.set@odatatype('#microsoft.graph.bookingWorkHours')

workingHours5.setDay@odatatype('#microsoft.graph.dayOfWeek')

workingHours5.setDay('friday')

workingHours5.setTimeSlots@odatatype('#Collection(microsoft.graph.bookingWorkTimeSlot)')

timeSlots1 = ()
timeSlots1.set@odatatype('#microsoft.graph.bookingWorkTimeSlot')

timeSlots1.setEndTime('17:00:00.0000000')

timeSlots1.setStartTime('08:00:00.0000000')


timeSlotsArray []= timeSlots1;
workingHours5.setTimeSlots(timeSlotsArray)



workingHoursArray []= workingHours5;
request_body.setWorkingHours(workingHoursArray)


];
request_body.setAdditionalData(additionalData)




result = await client.solutions.bookingBusinessesById('bookingBusiness-id').staffMembersById('bookingStaffMemberBase-id').patch(request_body)


```