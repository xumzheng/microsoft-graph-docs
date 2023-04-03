---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ForwardPostRequestBody();
toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setAddress('danas@contoso.onmicrosoft.com');

toRecipientsRecipient1EmailAddress.setName('Dana Swope');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);


requestBody.setComment('Dana, hope you can make this meeting.');



graphServiceClient.me().eventsById('event-id').forward().post(requestBody);


```