---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MessageRule();


$requestRequestBody->setDisplayName('From partner');
$requestRequestBody->setSequence(2);
$requestRequestBody->setIsEnabled(True);

$conditions = new MessageRulePredicates();
$requestRequestBody->setConditions($conditions);


$conditions->setSenderContains( [
'adele',],


$actions = new MessageRuleActions();
$requestRequestBody->setActions($actions);


$forwardToArray = [];

$forwardTo1 = new Recipient();


$emailAddress = new EmailAddress();
$forwardTo1->setEmailAddress($emailAddress);


$emailAddress->setName('Alex Wilbur');
$emailAddress->setAddress('AlexW@contoso.onmicrosoft.com');


$forwardToArray []= $forwardTo1;
$actions->setForwardTo($forwardToArray);
$actions->setStopProcessingRules(True);

$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->messageRules()->post($requestRequestBody);


```