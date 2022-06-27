---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Contact();


$requestRequestBody->setParentFolderId('parentFolderId-value');
$requestRequestBody->setBirthday(new DateTime("2016-10-19T10:37:00Z"));
$requestRequestBody->setFileAs('fileAs-value');
$requestRequestBody->setDisplayName('displayName-value');
$requestRequestBody->setGivenName('givenName-value');
$requestRequestBody->setInitials('initials-value');
$result =  $graphClient->me()->contactFoldersById('contactFolder-id')->contacts()->post($requestRequestBody);


```