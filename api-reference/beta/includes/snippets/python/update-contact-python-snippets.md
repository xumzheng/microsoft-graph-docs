---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Contact();
emailAddressesTypedEmailAddress1 = TypedEmailAddress();
emailAddressesTypedEmailAddress1.setType(EmailType('personal'));

emailAddressesTypedEmailAddress1.setName('Pavel Bansky');

emailAddressesTypedEmailAddress1.setAddress('pavelb@adatum.onmicrosoft.com');


emailAddressesArray []= emailAddressesTypedEmailAddress1;
emailAddressesTypedEmailAddress2 = TypedEmailAddress();
emailAddressesTypedEmailAddress2.setAddress('pavelb@fabrikam.onmicrosoft.com');

emailAddressesTypedEmailAddress2.setName('Pavel Bansky');

emailAddressesTypedEmailAddress2.setType(EmailType('other'));

emailAddressesTypedEmailAddress2.setOtherLabel('Volunteer work');


emailAddressesArray []= emailAddressesTypedEmailAddress2;
requestBody.setEmailAddresses(emailAddressesArray);




result = awaitclient.me().contactsById('contact-id').patch(requestBody);


```