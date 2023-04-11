---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
request_body.givenName = 'Pavel'

request_body.surname = 'Bansky'

emailAddressesTypedEmailAddress1 = TypedEmailAddress()
emailAddressesTypedEmailAddress1.address = 'pavelb@contoso.onmicrosoft.com'

emailAddressesTypedEmailAddress1.name = 'Pavel Bansky'

emailAddressesTypedEmailAddress1.Type(EmailType('personal'))


emailAddressesArray []= emailAddressesTypedEmailAddress1;
emailAddressesTypedEmailAddress2 = TypedEmailAddress()
emailAddressesTypedEmailAddress2.address = 'pavelb@fabrikam.onmicrosoft.com'

emailAddressesTypedEmailAddress2.name = 'Pavel Bansky'

emailAddressesTypedEmailAddress2.Type(EmailType('other'))

emailAddressesTypedEmailAddress2.otherLabel = 'Volunteer work'


emailAddressesArray []= emailAddressesTypedEmailAddress2;
request_body.emailaddresses(emailAddressesArray)


phonesPhone1 = Phone()
phonesPhone1.number = '+1 732 555 0102'

phonesPhone1.Type(PhoneType('business'))


phonesArray []= phonesPhone1;
request_body.phones(phonesArray)




request_configuration = ContactsRequestBuilderPostRequestConfiguration(
)


result = await client.me.contacts.post(request_body = request_body)


```