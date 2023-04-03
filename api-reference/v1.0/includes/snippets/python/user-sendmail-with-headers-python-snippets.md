---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SendMailPostRequestBody();
message = Message();
message.setSubject('9/9/2018: concert');

messageBody = ItemBody();
messageBody.setContentType(BodyType('html'));

messageBody.setContent('The group represents Nevada.');


message.setBody($messageBody);
toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setAddress('AlexW@contoso.OnMicrosoft.com');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
message.setToRecipients(toRecipientsArray);


internetMessageHeadersInternetMessageHeader1 = InternetMessageHeader();
internetMessageHeadersInternetMessageHeader1.setName('x-custom-header-group-name');

internetMessageHeadersInternetMessageHeader1.setValue('Nevada');


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader1;
internetMessageHeadersInternetMessageHeader2 = InternetMessageHeader();
internetMessageHeadersInternetMessageHeader2.setName('x-custom-header-group-id');

internetMessageHeadersInternetMessageHeader2.setValue('NV001');


internetMessageHeadersArray []= internetMessageHeadersInternetMessageHeader2;
message.setInternetMessageHeaders(internetMessageHeadersArray);



requestBody.setMessage($message);


await client.me().sendMail().post(requestBody);


```