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

$workingHours1 = new BookingWorkHours();

$workingHours1->setDay(new DayOfWeek('monday'));
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();

$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
			"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
		];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours1->setTimeSlots($timeSlotsArray);
$workingHours1AdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingWorkHours',
	"day@odata.type" => '#microsoft.graph.dayOfWeek',
	"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours1->setAdditionalData($workingHours1AdditionalData);

$workingHoursArray []= $workingHours1;

$workingHours2 = new BookingWorkHours();

$workingHours2->setDay(new DayOfWeek('tuesday'));
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();

$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
	"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours2->setTimeSlots($timeSlotsArray);
$workingHours2AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours2->setAdditionalData($workingHours2AdditionalData);

$workingHoursArray []= $workingHours2;

$workingHours3 = new BookingWorkHours();

$workingHours3->setDay(new DayOfWeek('wednesday'));
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();

$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours3->setTimeSlots($timeSlotsArray);
$workingHours3AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours3->setAdditionalData($workingHours3AdditionalData);

$workingHoursArray []= $workingHours3;

$workingHours4 = new BookingWorkHours();

$workingHours4->setDay(new DayOfWeek('thursday'));
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();

$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours4->setTimeSlots($timeSlotsArray);
$workingHours4AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours4->setAdditionalData($workingHours4AdditionalData);

$workingHoursArray []= $workingHours4;

$workingHours5 = new BookingWorkHours();

$workingHours5->setDay(new DayOfWeek('friday'));
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();

$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours5->setTimeSlots($timeSlotsArray);
$workingHours5AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours5->setAdditionalData($workingHours5AdditionalData);

$workingHoursArray []= $workingHours5;
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