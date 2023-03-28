---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ReplyPostRequestBody();
$message = new Message();
$toRecipientsRecipient1 = new Recipient();
$toRecipientsRecipient1EmailAddress = new EmailAddress();
$toRecipientsRecipient1EmailAddress.setAddress('samanthab@contoso.onmicrosoft.com');

$toRecipientsRecipient1EmailAddress.setName('Samantha Booth');


$toRecipientsRecipient1.setEmailAddress($toRecipientsRecipient1EmailAddress);

$toRecipientsArray []= $toRecipientsRecipient1;
$toRecipientsRecipient2 = new Recipient();
$toRecipientsRecipient2EmailAddress = new EmailAddress();
$toRecipientsRecipient2EmailAddress.setAddress('randiw@contoso.onmicrosoft.com');

$toRecipientsRecipient2EmailAddress.setName('Randi Welch');


$toRecipientsRecipient2.setEmailAddress($toRecipientsRecipient2EmailAddress);

$toRecipientsArray []= $toRecipientsRecipient2;
$message.setToRecipients($toRecipientsArray);



$requestBody.setMessage($message);
$requestBody.setComment('Samantha, Randi, would you name the group please?');



$graphServiceClient.me().messagesById('message-id').reply().post($requestBody);


```