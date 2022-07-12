---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingStaffMember = {
	"@odata.type" : "#microsoft.graph.bookingStaffMember",
	colorIndex : 1,
	displayName : "Dana Swope",
	emailAddress : "danas@contoso.com",
	role : "externalGuest",
	timeZone : "America/Chicago",
	useBusinessHours : true,
	workingHours : [
		{
			day : "monday",
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
	isEmailNotificationEnabled : false,
	additionalData : {
		"role@odata.type" : "#microsoft.graph.bookingStaffRole",
		"workingHours@odata.type" : "#Collection(microsoft.graph.bookingWorkHours)",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").staffMembers.post(requestBody);
}


```