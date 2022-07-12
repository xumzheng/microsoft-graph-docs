---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingStaffMember = {
	workingHours : [
		{
			day : "monday",
			timeSlots : [
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : "tuesday",
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : "wednesday",
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : "thursday",
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			day : "friday",
			timeSlots : [
				{
					end : "17:00:00.0000000",
					start : "08:00:00.0000000",
					additionalData : {
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					},
				},
			],
			additionalData : {
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").staffMembersById("bookingStaffMember-id").patch(requestBody);
}


```