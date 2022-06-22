---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendMailPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$message->setSubject('Meet for lunch?');

$body = new ItemBody();
$message->setBody($body);


$body->setContentType(new BodyType('Text'));
$body->setContent('The new cafeteria is open.');

$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('meganb@contoso.onmicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$message->setToRecipients($toRecipientsArray);
$attachmentsArray = [];

$attachments1 = new Attachment();

$attachments1->setName('attachment.txt');
$attachments1->setContentType('text/plain');
$attachments1AdditionalData = [
"@odata.type" => '#microsoft.graph.fileAttachment',
"contentBytes" => 'SGVsbG8gV29ybGQh',
];
$attachments1->setAdditionalData($attachments1AdditionalData);

$attachmentsArray []= $attachments1;
$message->setAttachments($attachmentsArray);

$result =  $graphClient->me()->sendMail()->post($requestRequestBody);


```