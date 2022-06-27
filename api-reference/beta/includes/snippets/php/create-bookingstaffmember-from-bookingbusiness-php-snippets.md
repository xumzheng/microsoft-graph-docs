---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingStaffMember();


$requestRequestBody->setColorIndex(1);
$requestRequestBody->setDisplayName('Dana Swope');
$requestRequestBody->setEmailAddress('danas@contoso.com');
$requestRequestBody->setRole(new BookingStaffRole('externalGuest'));
$requestRequestBody->setTimeZone('America/Chicago');
$requestRequestBody->setUseBusinessHours(True);
$workingHoursArray = [];

$workingHoursworkingHours1 = new BookingWorkHours();

$workingHoursworkingHours1->setDay(new DayOfWeek('monday'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new BookingWorkTimeSlot();

$timeSlotstimeSlots1->setEnd(new Time("17:00:00.0000000"));
$timeSlotstimeSlots1->setStart(new Time("08:00:00.0000000"));
$timeSlotstimeSlots1AdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlotstimeSlots1->setAdditionalData($timeSlotstimeSlots1AdditionalData);

$timeSlotsArray []= $timeSlotstimeSlots1;
$workingHoursworkingHours1->setTimeSlots($timeSlotsArray);
$workingHoursworkingHours1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHoursworkingHours1->setAdditionalData($workingHoursworkingHours1AdditionalData);

$workingHoursArray []= $workingHoursworkingHours1;

$workingHoursworkingHours2 = new BookingWorkHours();

$workingHoursworkingHours2->setDay(new DayOfWeek('tuesday'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new BookingWorkTimeSlot();

$timeSlotstimeSlots1->setEnd(new Time("17:00:00.0000000"));
$timeSlotstimeSlots1->setStart(new Time("08:00:00.0000000"));
$timeSlotstimeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlotstimeSlots1->setAdditionalData($timeSlotstimeSlots1AdditionalData);

$timeSlotsArray []= $timeSlotstimeSlots1;
$workingHoursworkingHours2->setTimeSlots($timeSlotsArray);
$workingHoursworkingHours2AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHoursworkingHours2->setAdditionalData($workingHoursworkingHours2AdditionalData);

$workingHoursArray []= $workingHoursworkingHours2;

$workingHoursworkingHours3 = new BookingWorkHours();

$workingHoursworkingHours3->setDay(new DayOfWeek('wednesday'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new BookingWorkTimeSlot();

$timeSlotstimeSlots1->setEnd(new Time("17:00:00.0000000"));
$timeSlotstimeSlots1->setStart(new Time("08:00:00.0000000"));
$timeSlotstimeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlotstimeSlots1->setAdditionalData($timeSlotstimeSlots1AdditionalData);

$timeSlotsArray []= $timeSlotstimeSlots1;
$workingHoursworkingHours3->setTimeSlots($timeSlotsArray);
$workingHoursworkingHours3AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHoursworkingHours3->setAdditionalData($workingHoursworkingHours3AdditionalData);

$workingHoursArray []= $workingHoursworkingHours3;

$workingHoursworkingHours4 = new BookingWorkHours();

$workingHoursworkingHours4->setDay(new DayOfWeek('thursday'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new BookingWorkTimeSlot();

$timeSlotstimeSlots1->setEnd(new Time("17:00:00.0000000"));
$timeSlotstimeSlots1->setStart(new Time("08:00:00.0000000"));
$timeSlotstimeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlotstimeSlots1->setAdditionalData($timeSlotstimeSlots1AdditionalData);

$timeSlotsArray []= $timeSlotstimeSlots1;
$workingHoursworkingHours4->setTimeSlots($timeSlotsArray);
$workingHoursworkingHours4AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHoursworkingHours4->setAdditionalData($workingHoursworkingHours4AdditionalData);

$workingHoursArray []= $workingHoursworkingHours4;

$workingHoursworkingHours5 = new BookingWorkHours();

$workingHoursworkingHours5->setDay(new DayOfWeek('friday'));
$timeSlotsArray = [];

$timeSlotstimeSlots1 = new BookingWorkTimeSlot();

$timeSlotstimeSlots1->setEnd(new Time("17:00:00.0000000"));
$timeSlotstimeSlots1->setStart(new Time("08:00:00.0000000"));
$timeSlotstimeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlotstimeSlots1->setAdditionalData($timeSlotstimeSlots1AdditionalData);

$timeSlotsArray []= $timeSlotstimeSlots1;
$workingHoursworkingHours5->setTimeSlots($timeSlotsArray);
$workingHoursworkingHours5AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHoursworkingHours5->setAdditionalData($workingHoursworkingHours5AdditionalData);

$workingHoursArray []= $workingHoursworkingHours5;
$requestRequestBody->setWorkingHours($workingHoursArray);
$requestRequestBody->setIsEmailNotificationEnabled(False);
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.bookingStaffMember',
"role@odata.type" => '#microsoft.graph.bookingStaffRole',
"workingHours@odata.type" => '#Collection(microsoft.graph.bookingWorkHours)',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->bookingBusinessesById('bookingBusiness-id')->staffMembers()->post($requestRequestBody);


```