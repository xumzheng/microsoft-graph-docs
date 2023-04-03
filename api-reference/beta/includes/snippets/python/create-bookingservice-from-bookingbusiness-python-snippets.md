---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = BookingService();
requestBody.set@odatatype('#microsoft.graph.bookingService');

$requestBody.setDefaultDuration( \DateInterval('PT1H30M'));

defaultLocation = Location();
defaultLocation.set@odatatype('#microsoft.graph.location');

defaultLocationAddress = PhysicalAddress();
defaultLocationAddress.set@odatatype('#microsoft.graph.physicalAddress');

defaultLocationAddress.setCity('Buffalo');

defaultLocationAddress.setCountryOrRegion('USA');

defaultLocationAddress.setPostalCode('98052');

DefaultLocationAddress.setPostOfficeBox(null);

defaultLocationAddress.setState('NY');

defaultLocationAddress.setStreet('4567 First Street');

DefaultLocationAddress.setType(null);

additionalData = [
'type@odata.type' => '#microsoft.graph.physicalAddressType', 
];
defaultLocationAddress.setAdditionalData(additionalData);



defaultLocation.setAddress($defaultLocationAddress);
DefaultLocation.setCoordinates(null);

defaultLocation.setDisplayName('Contoso Lunch Delivery');

DefaultLocation.setLocationEmailAddress(null);

DefaultLocation.setLocationType(null);

DefaultLocation.setLocationUri(null);

DefaultLocation.setUniqueId(null);

DefaultLocation.setUniqueIdType(null);

additionalData = [
'locationType@odata.type' => '#microsoft.graph.locationType', 
'uniqueIdType@odata.type' => '#microsoft.graph.locationUniqueIdType', 
];
defaultLocation.setAdditionalData(additionalData);



requestBody.setDefaultLocation($defaultLocation);
requestBody.setDefaultPrice(10);

requestBody.setDefaultPriceType(BookingPriceType('fixedprice'));

defaultRemindersBookingReminder1 = BookingReminder();
defaultRemindersBookingReminder1.set@odatatype('#microsoft.graph.bookingReminder');

defaultRemindersBookingReminder1.setMessage('Please be reminded that this service is tomorrow.');

$defaultRemindersBookingReminder1.setOffset( \DateInterval('P1D'));

defaultRemindersBookingReminder1.setRecipients(BookingReminderRecipients('allattendees'));

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
defaultRemindersBookingReminder1.setAdditionalData(additionalData);



defaultRemindersArray []= defaultRemindersBookingReminder1;
requestBody.setDefaultReminders(defaultRemindersArray);


requestBody.setDescription('Individual bento box lunch delivery');

requestBody.setDisplayName('Bento');

requestBody.setIsLocationOnline(true);

requestBody.setSmsNotificationsEnabled(true);

requestBody.setLanguageTag('en-US');

requestBody.setIsHiddenFromCustomers(false);

requestBody.setNotes('Home-cooked special');

$requestBody.setPostBuffer( \DateInterval('PT10M'));

$requestBody.setPreBuffer( \DateInterval('PT5M'));

schedulingPolicy = BookingSchedulingPolicy();
schedulingPolicy.set@odatatype('#microsoft.graph.bookingSchedulingPolicy');

schedulingPolicy.setAllowStaffSelection(true);

$schedulingPolicy.setMaximumAdvance( \DateInterval('P10D'));

$schedulingPolicy.setMinimumLeadTime( \DateInterval('PT10H'));

schedulingPolicy.setSendConfirmationsToOwner(true);

$schedulingPolicy.setTimeSlotInterval( \DateInterval('PT1H'));


requestBody.setSchedulingPolicy($schedulingPolicy);
requestBody.setStaffMemberIds(['d90d1e8c-5cfe-48cf-a2d5-966267375b6a', '2f5f8794-0b29-45b5-b56a-2eb5ff7aa880', ]);

requestBody.setIsAnonymousJoinEnabled(false);

additionalData = [
'defaultPriceType@odata.type' => '#microsoft.graph.bookingPriceType', 
'defaultReminders@odata.type' => '#Collection(microsoft.graph.bookingReminder)', 
'staffMemberIds@odata.type' => '#Collection(String)', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.bookingBusinessesById('bookingBusiness-id').services().post(requestBody);


```