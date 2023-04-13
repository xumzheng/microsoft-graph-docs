---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BookingAppointment()
request_body.@odatatype = '#microsoft.graph.bookingAppointment'

request_body.customerTimeZone = 'America/Chicago'

request_body.sms_notifications_enabled = True

end_date_time = DateTimeTimeZone()
endDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

endDateTime.dateTime = '2018-05-01T12:30:00.0000000+00:00'

endDateTime.timeZone = 'UTC'


request_body.end_date_time = endDateTime
request_body.is_location_online = True

request_body.opt_out_of_customer_email = False

request_body.anonymousJoinWebUrl=null

request_body.postbuffer =  \DateInterval('PT10M')

request_body.prebuffer =  \DateInterval('PT5M')

request_body.price = 10

request_body.PriceType(BookingPriceType('fixedprice'))

reminders_booking_reminder1 = BookingReminder()
remindersBookingReminder1.@odatatype = '#microsoft.graph.bookingReminder'

remindersBookingReminder1.message = 'This service is tomorrow'

remindersBookingReminder1.offset =  \DateInterval('P1D')

remindersBookingReminder1.Recipients(BookingReminderRecipients('allattendees'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder1.additionaldata(additionalData)



remindersArray []= remindersBookingReminder1;
reminders_booking_reminder2 = BookingReminder()
remindersBookingReminder2.@odatatype = '#microsoft.graph.bookingReminder'

remindersBookingReminder2.message = 'Please be available to enjoy your lunch service.'

remindersBookingReminder2.offset =  \DateInterval('PT1H')

remindersBookingReminder2.Recipients(BookingReminderRecipients('customer'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder2.additionaldata(additionalData)



remindersArray []= remindersBookingReminder2;
reminders_booking_reminder3 = BookingReminder()
remindersBookingReminder3.@odatatype = '#microsoft.graph.bookingReminder'

remindersBookingReminder3.message = 'Please check traffic for next cater.'

remindersBookingReminder3.offset =  \DateInterval('PT2H')

remindersBookingReminder3.Recipients(BookingReminderRecipients('staff'))

additionalData = [
'recipients@odata.type' => '#microsoft.graph.bookingReminderRecipients', 
];
remindersBookingReminder3.additionaldata(additionalData)



remindersArray []= remindersBookingReminder3;
request_body.reminders(remindersArray)


request_body.serviceId = '57da6774-a087-4d69-b0e6-6fb82c339976'

service_location = Location()
serviceLocation.@odatatype = '#microsoft.graph.location'

service_location_address = PhysicalAddress()
serviceLocationAddress.@odatatype = '#microsoft.graph.physicalAddress'

serviceLocationAddress.city = 'Buffalo'

serviceLocationAddress.countryOrRegion = 'USA'

serviceLocationAddress.postalCode = '98052'

serviceLocationAddress.state = 'NY'

serviceLocationAddress.street = '123 First Avenue'

additionalData = [
'postOfficeBox' => 	null,
'type@odata.type' => '#microsoft.graph.physicalAddressType', 
'type' => 	null,
];
serviceLocationAddress.additionaldata(additionalData)



serviceLocation.address = serviceLocationAddress
ServiceLocation.coordinates=null

serviceLocation.displayName = 'Customer location'

ServiceLocation.locationEmailAddress=null

ServiceLocation.locationType=null

ServiceLocation.locationUri=null

ServiceLocation.uniqueId=null

ServiceLocation.uniqueIdType=null

additionalData = [
'locationType@odata.type' => '#microsoft.graph.locationType', 
'uniqueIdType@odata.type' => '#microsoft.graph.locationUniqueIdType', 
];
serviceLocation.additionaldata(additionalData)



request_body.service_location = serviceLocation
request_body.serviceName = 'Catered bento'

request_body.serviceNotes = 'Customer requires punctual service.'

start_date_time = DateTimeTimeZone()
startDateTime.@odatatype = '#microsoft.graph.dateTimeTimeZone'

startDateTime.dateTime = '2018-05-01T12:00:00.0000000+00:00'

startDateTime.timeZone = 'UTC'


request_body.start_date_time = startDateTime
request_body.maximum_attendees_count = 5

request_body.filled_attendees_count = 1

customers_booking_customer_information_base1 = BookingCustomerInformationBase()
customersBookingCustomerInformationBase1.@odatatype = '#microsoft.graph.bookingCustomerInformation'

additionalData = [
'customerId' => '7ed53fa5-9ef2-4f2f-975b-27447440bc09', 
'name' => 'Jordan Miller', 
'emailAddress' => 'jordanm@contoso.com', 
'phone' => '213-555-0199', 
'notes' => 	null,
'location' => customers_booking_customer_information_base1 = Location()
	customersBookingCustomerInformationBase1.@odatatype = '#microsoft.graph.location'

	customersBookingCustomerInformationBase1.displayName = 'Customer'

	customersBookingCustomerInformationBase1.locationEmailAddress=null

	customersBookingCustomerInformationBase1.locationUri = ''

	customersBookingCustomerInformationBase1.locationType=null

	customersBookingCustomerInformationBase1.uniqueId=null

	customersBookingCustomerInformationBase1.uniqueIdType=null

address = Address()
	address.@odatatype = '#microsoft.graph.physicalAddress'

	address.street = ''

	address.city = ''

	address.state = ''

	address.countryOrRegion = ''

	address.postalCode = ''


customersBookingCustomerInformationBase1.address = address
coordinates = Coordinates()
	Coordinates.altitude=null

	Coordinates.latitude=null

	Coordinates.longitude=null

	Coordinates.accuracy=null

	Coordinates.altitudeAccuracy=null


customersBookingCustomerInformationBase1.coordinates = coordinates

customersBookingCustomerInformationBase1.location = location

'timeZone' => 'America/Chicago', 
'customQuestionAnswers' => custom_question_answers1 = ()
	customQuestionAnswers1.questionId = '3bc6fde0-4ad3-445d-ab17-0fc15dba0774'

	customQuestionAnswers1.question = 'What is your age?'

	customQuestionAnswers1.answerInputType = 'text'

customQuestionAnswers1.AnswerOptions([])

customQuestionAnswers1.is_required = True

customQuestionAnswers1.answer = '25'

customQuestionAnswers1.SelectedOptions([])


customQuestionAnswersArray []= customQuestionAnswers1;
customersBookingCustomerInformationBase1.customquestionanswers(customQuestionAnswersArray)


];
customersBookingCustomerInformationBase1.additionaldata(additionalData)



customersArray []= customersBookingCustomerInformationBase1;
request_body.customers(customersArray)


additionalData = [
'priceType@odata.type' => '#microsoft.graph.bookingPriceType', 
'reminders@odata.type' => '#Collection(microsoft.graph.bookingReminder)', 
'customers@odata.type' => '#Collection(microsoft.graph.bookingCustomerInformation)', 
];
request_body.additionaldata(additionalData)





result = await client.solutions.bookingBusinesses_by_id('bookingBusiness-id').appointments.post(request_body = request_body)


```