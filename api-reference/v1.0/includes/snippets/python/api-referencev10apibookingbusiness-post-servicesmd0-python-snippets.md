---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingService()
request_body.set@odatatype('#microsoft.graph.bookingService')

$request_body.setDefaultDuration( \DateInterval('PT1H30M'))

defaultLocation = Location()
defaultLocation.set@odatatype('#microsoft.graph.location')

defaultLocationAddress = PhysicalAddress()
defaultLocationAddress.set@odatatype('#microsoft.graph.physicalAddress')

defaultLocationAddress.setCity('Buffalo')

defaultLocationAddress.setCountryOrRegion('USA')

defaultLocationAddress.setPostalCode('98052')

defaultLocationAddress.setState('NY')

defaultLocationAddress.setStreet('4567 First Street')

additionalData = [
'postOfficeBox' => 		null,
'type@odata.type' => '#microsoft.graph.physicalAddressType', 
'type' => 		null,
];
defaultLocationAddress.setAdditionalData(additionalData)



defaultLocation.setAddress($defaultLocationAddress)
DefaultLocation.setCoordinates(null)

defaultLocation.setDisplayName('Contoso Lunch Delivery')

DefaultLocation.setLocationEmailAddress(null)

DefaultLocation.setLocationType(null)

DefaultLocation.setLocationUri(null)

DefaultLocation.setUniqueId(null)

DefaultLocation.setUniqueIdType(null)

additionalData = [
'locationType@odata.type' => '#microsoft.graph.locationType', 
'uniqueIdType@odata.type' => '#microsoft.graph.locationUniqueIdType', 
];
defaultLocation.setAdditionalData(additionalData)



request_body.setDefaultLocation($defaultLocation)
request_body.setDefaultPrice(10)

request_body.setDefaultPriceType(BookingPriceType('fixedprice'))

defaultRemindersBookingReminder1 = BookingReminder()
defaultRemindersBookingReminder1.set@odatatype('#microsoft.graph.bookingReminder')

defaultRemindersBookingReminder1.setMessage('Please be reminded that this service is tomorrow.')

$defaultRemindersBookingReminder1.setOffset( \DateInterval('P1D'))

defaultRemindersBookingReminder1.setRecipients(BookingReminderRecipients('allattendees'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
defaultRemindersBookingReminder1.setAdditionalData(additionalData)



defaultRemindersArray []= defaultRemindersBookingReminder1;
request_body.setDefaultReminders(defaultRemindersArray)


request_body.setDescription('Individual bento box lunch delivery')

request_body.setDisplayName('Bento')

request_body.setIsLocationOnline(true)

request_body.setSmsNotificationsEnabled(true)

request_body.setLanguageTag('en-US')

request_body.setIsHiddenFromCustomers(false)

request_body.setNotes('Home-cooked special')

$request_body.setPostBuffer( \DateInterval('PT10M'))

$request_body.setPreBuffer( \DateInterval('PT5M'))

schedulingPolicy = BookingSchedulingPolicy()
schedulingPolicy.set@odatatype('#microsoft.graph.bookingSchedulingPolicy')

schedulingPolicy.setAllowStaffSelection(true)

$schedulingPolicy.setMaximumAdvance( \DateInterval('P10D'))

$schedulingPolicy.setMinimumLeadTime( \DateInterval('PT10H'))

schedulingPolicy.setSendConfirmationsToOwner(true)

$schedulingPolicy.setTimeSlotInterval( \DateInterval('PT1H'))


request_body.setSchedulingPolicy($schedulingPolicy)
request_body.setStaffMemberIds(['d90d1e8c-5cfe-48cf-a2d5-966267375b6a', '2f5f8794-0b29-45b5-b56a-2eb5ff7aa880', ])

request_body.setIsAnonymousJoinEnabled(false)

additionalData = [
'defaultPriceType@odata.type' => '#microsoft.graph.bookingPriceType', 
'defaultReminders@odata.type' => '#Collection(microsoft.graph.bookingReminder)', 
'staffMemberIds@odata.type' => '#Collection(String)', 
];
request_body.setAdditionalData(additionalData)




result = await client.solutions.bookingBusinesses._by_id('bookingBusiness-id').services.post(request_body)


```