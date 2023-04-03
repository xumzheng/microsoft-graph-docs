---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Message();
requestBody.setSubject('9/8/2018: concert');

body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('The group represents Washington.');


requestBody.setBody($body);
toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setAddress('AlexW@contoso.OnMicrosoft.com');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);


internetMessageHeadersInternetMessageHeader1 = InternetMessageHeader();
internetMessageHeadersInternetMessageHeader1.setName('x-custom-header-group-name');

internetMessageHeadersInternetMessageHeader1.setValue('Washington');


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader1;
internetMessageHeadersInternetMessageHeader2 = InternetMessageHeader();
internetMessageHeadersInternetMessageHeader2.setName('x-custom-header-group-id');

internetMessageHeadersInternetMessageHeader2.setValue('WA001');


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader2;
requestBody.setInternetMessageHeaders(internetMessageHeadersArray);




result = awaitclient.me().messages().post(requestBody);


```