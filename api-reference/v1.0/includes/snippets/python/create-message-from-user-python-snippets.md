---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Message();
requestBody.setSubject('Did you see last night\'s game?');

requestBody.setImportance(Importance('low'));

body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('They were <b>awesome</b>!');


requestBody.setBody($body);
toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setAddress('AdeleV@contoso.onmicrosoft.com');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);




result = awaitclient.me().messages().post(requestBody);


```