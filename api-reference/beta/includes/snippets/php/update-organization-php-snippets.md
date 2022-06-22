---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Organization();


$requestRequestBody->setMarketingNotificationEmails( [
'marketing@contoso.com',],

$privacyProfile = new PrivacyProfile();
$requestRequestBody->setPrivacyProfile($privacyProfile);


$privacyProfile->setContactEmail('alice@contoso.com');
$privacyProfile->setStatementUrl('https://contoso.com/privacyStatement');

$requestRequestBody->setSecurityComplianceNotificationMails( [
'security@contoso.com',],
$requestRequestBody->setSecurityComplianceNotificationPhones( [
'(123) 456-7890',],
$requestRequestBody->setTechnicalNotificationMails( [
'tech@contoso.com',],
$result =  $graphClient->organizationById('organization-id')->patch($requestRequestBody);


```