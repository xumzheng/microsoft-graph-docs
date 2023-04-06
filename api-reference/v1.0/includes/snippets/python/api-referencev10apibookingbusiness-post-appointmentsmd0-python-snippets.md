---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.set@odatatype('#microsoft.graph.bookingAppointment')

request_body.setCustomerTimeZone('America/Chicago')

request_body.setSmsNotificationsEnabled(true)

endDateTime = DateTimeTimeZone()
endDateTime.set@odatatype('#microsoft.graph.dateTimeTimeZone')

endDateTime.setDateTime('2018-05-01T12:30:00.0000000+00:00')

endDateTime.setTimeZone('UTC')


request_body.setEndDateTime($endDateTime)
request_body.setIsLocationOnline(true)

request_body.setOptOutOfCustomerEmail(false)

request_body.setAnonymousJoinWebUrl(null)

$request_body.setPostBuffer( \DateInterval('PT10M'))

$request_body.setPreBuffer( \DateInterval('PT5M'))

request_body.setPrice(10)

request_body.setPriceType(BookingPriceType('fixedprice'))

remindersBookingReminder1 = BookingReminder()
remindersBookingReminder1.set@odatatype('#microsoft.graph.bookingReminder')

remindersBookingReminder1.setMessage('This service is tomorrow')

$remindersBookingReminder1.setOffset( \DateInterval('P1D'))

remindersBookingReminder1.setRecipients(BookingReminderRecipients('allattendees'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder1.setAdditionalData(additionalData)



remindersArray []= remindersBookingReminder1;
remindersBookingReminder2 = BookingReminder()
remindersBookingReminder2.set@odatatype('#microsoft.graph.bookingReminder')

remindersBookingReminder2.setMessage('Please be available to enjoy your lunch service.')

$remindersBookingReminder2.setOffset( \DateInterval('PT1H'))

remindersBookingReminder2.setRecipients(BookingReminderRecipients('customer'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder2.setAdditionalData(additionalData)



remindersArray []= remindersBookingReminder2;
remindersBookingReminder3 = BookingReminder()
remindersBookingReminder3.set@odatatype('#microsoft.graph.bookingReminder')

remindersBookingReminder3.setMessage('Please check traffic for next cater.')

$remindersBookingReminder3.setOffset( \DateInterval('PT2H'))

remindersBookingReminder3.setRecipients(BookingReminderRecipients('staff'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder3.setAdditionalData(additionalData)



remindersArray []= remindersBookingReminder3;
request_body.setReminders(remindersArray)


request_body.setServiceId('57da6774-a087-4d69-b0e6-6fb82c339976')

serviceLocation = Location()
serviceLocation.set@odatatype('#microsoft.graph.location')

serviceLocationAddress = PhysicalAddress()
serviceLocationAddress.set@odatatype('#microsoft.graph.physicalAddress')

serviceLocationAddress.setCity('Buffalo')

serviceLocationAddress.setCountryOrRegion('USA')

serviceLocationAddress.setPostalCode('98052')

serviceLocationAddress.setState('NY')

serviceLocationAddress.setStreet('123 First Avenue')

additionalData = [
'postOfficeBox' => 	null,
'type@odata.type' => '#microsoft.graph.physicalAddressType', 
'type' => 	null,
];
serviceLocationAddress.setAdditionalData(additionalData)



serviceLocation.setAddress($serviceLocationAddress)
ServiceLocation.setCoordinates(null)

serviceLocation.setDisplayName('Customer location')

ServiceLocation.setLocationEmailAddress(null)

ServiceLocation.setLocationType(null)

ServiceLocation.setLocationUri(null)

ServiceLocation.setUniqueId(null)

ServiceLocation.setUniqueIdType(null)

additionalData = [
'locationType@odata.type' => '#microsoft.graph.locationType', 
'uniqueIdType@odata.type' => '#microsoft.graph.locationUniqueIdType', 
];
serviceLocation.setAdditionalData(additionalData)



request_body.setServiceLocation($serviceLocation)
request_body.setServiceName('Catered bento')

request_body.setServiceNotes('Customer requires punctual service.')

startDateTime = DateTimeTimeZone()
startDateTime.set@odatatype('#microsoft.graph.dateTimeTimeZone')

startDateTime.setDateTime('2018-05-01T12:00:00.0000000+00:00')

startDateTime.setTimeZone('UTC')


request_body.setStartDateTime($startDateTime)
request_body.setMaximumAttendeesCount(5)

request_body.setFilledAttendeesCount(1)

customersBookingCustomerInformationBase1 = BookingCustomerInformationBase()
customersBookingCustomerInformationBase1.set@odatatype('#microsoft.graph.bookingCustomerInformation')

additionalData = [
'customerId' => '7ed53fa5-9ef2-4f2f-975b-27447440bc09', 
'name' => 'Jordan Miller', 
'emailAddress' => 'jordanm@contoso.com', 
'phone' => '213-555-0199', 
'notes' => 	null,
'location' => customersBookingCustomerInformationBase1 = Location()
	customersBookingCustomerInformationBase1.set@odatatype('#microsoft.graph.location')

	customersBookingCustomerInformationBase1.setDisplayName('Customer')

	customersBookingCustomerInformationBase1.setLocationEmailAddress(null)

	customersBookingCustomerInformationBase1.setLocationUri('')

	customersBookingCustomerInformationBase1.setLocationType(null)

	customersBookingCustomerInformationBase1.setUniqueId(null)

	customersBookingCustomerInformationBase1.setUniqueIdType(null)

address = Address()
	address.set@odatatype('#microsoft.graph.physicalAddress')

	address.setStreet('')

	address.setCity('')

	address.setState('')

	address.setCountryOrRegion('')

	address.setPostalCode('')


customersBookingCustomerInformationBase1.setAddress($address)
coordinates = Coordinates()
	Coordinates.setAltitude(null)

	Coordinates.setLatitude(null)

	Coordinates.setLongitude(null)

	Coordinates.setAccuracy(null)

	Coordinates.setAltitudeAccuracy(null)


customersBookingCustomerInformationBase1.setCoordinates($coordinates)

customersBookingCustomerInformationBase1.setLocation($location)

'timeZone' => 'America/Chicago', 
'customQuestionAnswers' => customQuestionAnswers1 = ()
	customQuestionAnswers1.setQuestionId('3bc6fde0-4ad3-445d-ab17-0fc15dba0774')

	customQuestionAnswers1.setQuestion('What is your age?')

	customQuestionAnswers1.setAnswerInputType('text')

customQuestionAnswers1.setAnswerOptions([])

customQuestionAnswers1.setIsRequired(true)

customQuestionAnswers1.setAnswer('25')

customQuestionAnswers1.setSelectedOptions([])


customQuestionAnswersArray []= customQuestionAnswers1;
customersBookingCustomerInformationBase1.setCustomQuestionAnswers(customQuestionAnswersArray)


];
customersBookingCustomerInformationBase1.setAdditionalData(additionalData)



customersArray []= customersBookingCustomerInformationBase1;
request_body.setCustomers(customersArray)


additionalData = [
'priceType@odata.type' => '#microsoft.graph.bookingPriceType', 
'reminders@odata.type' => '#Collection(microsoft.graph.bookingReminder)', 
'customers@odata.type' => '#Collection(microsoft.graph.bookingCustomerInformation)', 
];
request_body.setAdditionalData(additionalData)




result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').appointments.post(request_body, headers=)


```