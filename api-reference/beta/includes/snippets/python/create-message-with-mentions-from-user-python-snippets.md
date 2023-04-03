---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Message();
requestBody.setSubject('Party planning');

toRecipientsRecipient1 = Recipient();
toRecipientsRecipient1EmailAddress = EmailAddress();
toRecipientsRecipient1EmailAddress.setName('Samantha Booth');

toRecipientsRecipient1EmailAddress.setAddress('samanthab@contoso.onmicrosoft.com');


toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

toRecipientsArray []= toRecipientsRecipient1;
requestBody.setToRecipients(toRecipientsArray);


mentionsMention1 = Mention();
mentionsMention1Mentioned = EmailAddress();
mentionsMention1Mentioned.setName('Dana Swope');

mentionsMention1Mentioned.setAddress('danas@contoso.onmicrosoft.com');


mentionsMention1.setMentioned($mentionsMention1Mentioned);

mentionsArray []= mentionsMention1;
requestBody.setMentions(mentionsArray);




requestResult = graphServiceClient.me().messages().post(requestBody);


```