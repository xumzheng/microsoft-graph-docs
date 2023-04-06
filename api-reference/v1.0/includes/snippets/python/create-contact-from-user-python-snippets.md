---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
request_body.setGivenName('Pavel')

request_body.setSurname('Bansky')

emailAddressesEmailAddress1 = EmailAddress()
emailAddressesEmailAddress1.setAddress('pavelb@fabrikam.onmicrosoft.com')

emailAddressesEmailAddress1.setName('Pavel Bansky')


emailAddressesArray []= emailAddressesEmailAddress1;
request_body.setEmailAddresses(emailAddressesArray)


request_body.setBusinessPhones(['+1 732 555 0102', ])



result = await client.me.contacts.post(request_body, headers=)


```