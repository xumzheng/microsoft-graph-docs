---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingStaffMemberBase()
request_body.@odatatype = '#microsoft.graph.bookingStaffMember'

additionalData = [
'workingHours' => workingHours1 = ()
		workingHours1.@odatatype = '#microsoft.graph.bookingWorkHours'

		workingHours1.day@odatatype = '#microsoft.graph.dayOfWeek'

		workingHours1.day = 'monday'

		workingHours1.timeSlots@odatatype = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

workingHours1.TimeSlots([])


workingHoursArray []= workingHours1;
workingHours2 = ()
	workingHours2.@odatatype = '#microsoft.graph.bookingWorkHours'

	workingHours2.day@odatatype = '#microsoft.graph.dayOfWeek'

	workingHours2.day = 'tuesday'

	workingHours2.timeSlots@odatatype = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

timeSlots1 = ()
	timeSlots1.@odatatype = '#microsoft.graph.bookingWorkTimeSlot'

	timeSlots1.endTime = '17:00:00.0000000'

	timeSlots1.startTime = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
workingHours2.timeslots(timeSlotsArray)



workingHoursArray []= workingHours2;
workingHours3 = ()
workingHours3.@odatatype = '#microsoft.graph.bookingWorkHours'

workingHours3.day@odatatype = '#microsoft.graph.dayOfWeek'

workingHours3.day = 'wednesday'

workingHours3.timeSlots@odatatype = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

timeSlots1 = ()
timeSlots1.@odatatype = '#microsoft.graph.bookingWorkTimeSlot'

timeSlots1.endTime = '17:00:00.0000000'

timeSlots1.startTime = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
workingHours3.timeslots(timeSlotsArray)



workingHoursArray []= workingHours3;
workingHours4 = ()
workingHours4.@odatatype = '#microsoft.graph.bookingWorkHours'

workingHours4.day@odatatype = '#microsoft.graph.dayOfWeek'

workingHours4.day = 'thursday'

workingHours4.timeSlots@odatatype = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

timeSlots1 = ()
timeSlots1.@odatatype = '#microsoft.graph.bookingWorkTimeSlot'

timeSlots1.endTime = '17:00:00.0000000'

timeSlots1.startTime = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
workingHours4.timeslots(timeSlotsArray)



workingHoursArray []= workingHours4;
workingHours5 = ()
workingHours5.@odatatype = '#microsoft.graph.bookingWorkHours'

workingHours5.day@odatatype = '#microsoft.graph.dayOfWeek'

workingHours5.day = 'friday'

workingHours5.timeSlots@odatatype = '#Collection(microsoft.graph.bookingWorkTimeSlot)'

timeSlots1 = ()
timeSlots1.@odatatype = '#microsoft.graph.bookingWorkTimeSlot'

timeSlots1.endTime = '17:00:00.0000000'

timeSlots1.startTime = '08:00:00.0000000'


timeSlotsArray []= timeSlots1;
workingHours5.timeslots(timeSlotsArray)



workingHoursArray []= workingHours5;
request_body.workinghours(workingHoursArray)


];
request_body.additionaldata(additionalData)





result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').staffMembers_by_id('bookingStaffMemberBase-id').patch(request_body = request_body)


```