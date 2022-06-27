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

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('meganb@contoso.onmicrosoft.com');


$toRecipientsArray []= $toRecipientstoRecipients1;
$message->setToRecipients($toRecipientsArray);
$attachmentsArray = [];

$attachmentsattachments1 = new Attachment();

$attachmentsattachments1->setName('attachment.txt');
$attachmentsattachments1->setContentType('text/plain');
$attachmentsattachments1AdditionalData = [
"@odata.type" => '#microsoft.graph.fileAttachment',
"contentBytes" => 'SGVsbG8gV29ybGQh',
];
$attachmentsattachments1->setAdditionalData($attachmentsattachments1AdditionalData);

$attachmentsArray []= $attachmentsattachments1;
$message->setAttachments($attachmentsArray);

$result =  $graphClient->me()->sendMail()->post($requestRequestBody);


```