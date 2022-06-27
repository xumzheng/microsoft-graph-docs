---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Message();


$requestRequestBody->setSubject('Annual review');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('You should be proud!');

$toRecipientsArray = [];

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('rufus@contoso.com');


$toRecipientsArray []= $toRecipientstoRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$extensionsArray = [];

$extensionsextensions1 = new Extension();

$extensionsextensions1AdditionalData = [
"@odata.type" => 'microsoft.graph.openTypeExtension',
"extensionName" => 'Com.Contoso.Referral',
"companyName" => 'Wingtip Toys',
"expirationDate" => '2015-12-30T11:00:00.000Z',
"dealValue" => 10000,
];
$extensionsextensions1->setAdditionalData($extensionsextensions1AdditionalData);

$extensionsArray []= $extensionsextensions1;
$requestRequestBody->setExtensions($extensionsArray);
$result =  $graphClient->me()->messages()->post($requestRequestBody);


```