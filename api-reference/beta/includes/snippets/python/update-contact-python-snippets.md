---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
emailAddressesTypedEmailAddress1 = TypedEmailAddress()
emailAddressesTypedEmailAddress1.Type(EmailType('personal'))

emailAddressesTypedEmailAddress1.name = 'Pavel Bansky'

emailAddressesTypedEmailAddress1.address = 'pavelb@adatum.onmicrosoft.com'


emailAddressesArray []= emailAddressesTypedEmailAddress1;
emailAddressesTypedEmailAddress2 = TypedEmailAddress()
emailAddressesTypedEmailAddress2.address = 'pavelb@fabrikam.onmicrosoft.com'

emailAddressesTypedEmailAddress2.name = 'Pavel Bansky'

emailAddressesTypedEmailAddress2.Type(EmailType('other'))

emailAddressesTypedEmailAddress2.otherLabel = 'Volunteer work'


emailAddressesArray []= emailAddressesTypedEmailAddress2;
request_body.emailaddresses(emailAddressesArray)





result = await client.me.contacts_by_id('contact-id').patch(request_body = request_body)


```