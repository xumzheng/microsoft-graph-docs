---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingService()
request_body.@odatatype = '#microsoft.graph.bookingService'

request_body.defaultduration =  \DateInterval('PT1H30M')

defaultLocation = Location()
defaultLocation.@odatatype = '#microsoft.graph.location'

defaultLocationAddress = PhysicalAddress()
defaultLocationAddress.@odatatype = '#microsoft.graph.physicalAddress'

defaultLocationAddress.city = 'Buffalo'

defaultLocationAddress.countryOrRegion = 'USA'

defaultLocationAddress.postalCode = '98052'

defaultLocationAddress.state = 'NY'

defaultLocationAddress.street = '4567 First Street'

additionalData = [
'postOfficeBox' => 		null,
'type@odata.type' => '#microsoft.graph.physicalAddressType', 
'type' => 		null,
];
defaultLocationAddress.additionaldata(additionalData)



defaultLocation.address = defaultLocationAddress
DefaultLocation.coordinates=null

defaultLocation.displayName = 'Contoso Lunch Delivery'

DefaultLocation.locationEmailAddress=null

DefaultLocation.locationType=null

DefaultLocation.locationUri=null

DefaultLocation.uniqueId=null

DefaultLocation.uniqueIdType=null

additionalData = [
'locationType@odata.type' => '#microsoft.graph.locationType', 
'uniqueIdType@odata.type' => '#microsoft.graph.locationUniqueIdType', 
];
defaultLocation.additionaldata(additionalData)



request_body.defaultLocation = defaultLocation
request_body.defaultPrice = 10

request_body.DefaultPriceType(BookingPriceType('fixedprice'))

defaultRemindersBookingReminder1 = BookingReminder()
defaultRemindersBookingReminder1.@odatatype = '#microsoft.graph.bookingReminder'

defaultRemindersBookingReminder1.message = 'Please be reminded that this service is tomorrow.'

defaultRemindersBookingReminder1.offset =  \DateInterval('P1D')

defaultRemindersBookingReminder1.Recipients(BookingReminderRecipients('allattendees'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
defaultRemindersBookingReminder1.additionaldata(additionalData)



defaultRemindersArray []= defaultRemindersBookingReminder1;
request_body.defaultreminders(defaultRemindersArray)


request_body.description = 'Individual bento box lunch delivery'

request_body.displayName = 'Bento'

request_body.isLocationOnline = true

request_body.smsNotificationsEnabled = true

request_body.languageTag = 'en-US'

request_body.isHiddenFromCustomers = false

request_body.notes = 'Home-cooked special'

request_body.postbuffer =  \DateInterval('PT10M')

request_body.prebuffer =  \DateInterval('PT5M')

schedulingPolicy = BookingSchedulingPolicy()
schedulingPolicy.@odatatype = '#microsoft.graph.bookingSchedulingPolicy'

schedulingPolicy.allowStaffSelection = true

schedulingPolicy.maximumadvance =  \DateInterval('P10D')

schedulingPolicy.minimumleadtime =  \DateInterval('PT10H')

schedulingPolicy.sendConfirmationsToOwner = true

schedulingPolicy.timeslotinterval =  \DateInterval('PT1H')


request_body.schedulingPolicy = schedulingPolicy
request_body.StaffMemberIds(['d90d1e8c-5cfe-48cf-a2d5-966267375b6a', '2f5f8794-0b29-45b5-b56a-2eb5ff7aa880', ])

request_body.isAnonymousJoinEnabled = false

additionalData = [
'defaultPriceType@odata.type' => '#microsoft.graph.bookingPriceType', 
'defaultReminders@odata.type' => '#Collection(microsoft.graph.bookingReminder)', 
'staffMemberIds@odata.type' => '#Collection(String)', 
];
request_body.additionaldata(additionalData)




request_configuration = ServicesRequestBuilderPostRequestConfiguration(
)


result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').services.post(request_body = request_body)


```