---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Contact();
requestBody.setGivenName('Pavel');

requestBody.setSurname('Bansky');

emailAddressesTypedEmailAddress1 = TypedEmailAddress();
emailAddressesTypedEmailAddress1.setAddress('pavelb@contoso.onmicrosoft.com');

emailAddressesTypedEmailAddress1.setName('Pavel Bansky');

emailAddressesTypedEmailAddress1.setType(EmailType('personal'));


emailAddressesArray []= emailAddressesTypedEmailAddress1;
emailAddressesTypedEmailAddress2 = TypedEmailAddress();
emailAddressesTypedEmailAddress2.setAddress('pavelb@fabrikam.onmicrosoft.com');

emailAddressesTypedEmailAddress2.setName('Pavel Bansky');

emailAddressesTypedEmailAddress2.setType(EmailType('other'));

emailAddressesTypedEmailAddress2.setOtherLabel('Volunteer work');


emailAddressesArray []= emailAddressesTypedEmailAddress2;
requestBody.setEmailAddresses(emailAddressesArray);


phonesPhone1 = Phone();
phonesPhone1.setNumber('+1 732 555 0102');

phonesPhone1.setType(PhoneType('business'));


phonesArray []= phonesPhone1;
requestBody.setPhones(phonesArray);




result = await client.me().contacts().post(requestBody);


```