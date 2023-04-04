---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Contact()
request_body.setGivenName('Pavel')

request_body.setSurname('Bansky')

emailAddressesTypedEmailAddress1 = TypedEmailAddress()
emailAddressesTypedEmailAddress1.setAddress('pavelb@contoso.onmicrosoft.com')

emailAddressesTypedEmailAddress1.setName('Pavel Bansky')

emailAddressesTypedEmailAddress1.setType(EmailType('personal'))


emailAddressesArray []= emailAddressesTypedEmailAddress1;
emailAddressesTypedEmailAddress2 = TypedEmailAddress()
emailAddressesTypedEmailAddress2.setAddress('pavelb@fabrikam.onmicrosoft.com')

emailAddressesTypedEmailAddress2.setName('Pavel Bansky')

emailAddressesTypedEmailAddress2.setType(EmailType('other'))

emailAddressesTypedEmailAddress2.setOtherLabel('Volunteer work')


emailAddressesArray []= emailAddressesTypedEmailAddress2;
request_body.setEmailAddresses(emailAddressesArray)


phonesPhone1 = Phone()
phonesPhone1.setNumber('+1 732 555 0102')

phonesPhone1.setType(PhoneType('business'))


phonesArray []= phonesPhone1;
request_body.setPhones(phonesArray)




result = await client.me.contacts.post(request_body)


```