---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContentType();


$requestRequestBody->setName('updatedCt');

$documentSet = new DocumentSet();
$requestRequestBody->setDocumentSet($documentSet);


$documentSet->setShouldPrefixNameToFile(True);
$allowedContentTypesArray = [];

$allowedContentTypes1 = new ContentTypeInfo();

$allowedContentTypes1->setId('0x0101');
$allowedContentTypes1->setName('Document');

$allowedContentTypesArray []= $allowedContentTypes1;
$documentSet->setAllowedContentTypes($allowedContentTypesArray);
$defaultContentsArray = [];

$defaultContents1 = new DocumentSetContent();

$defaultContents1->setFileName('a.txt');

$contentType = new ContentTypeInfo();
$defaultContents1->setContentType($contentType);


$contentType->setId('0x0101');


$defaultContentsArray []= $defaultContents1;

$defaultContents2 = new DocumentSetContent();

$defaultContents2->setFileName('b.txt');

$contentType = new ContentTypeInfo();
$defaultContents2->setContentType($contentType);


$contentType->setId('0x0101');


$defaultContentsArray []= $defaultContents2;
$documentSet->setDefaultContents($defaultContentsArray);
$sharedColumnsArray = [];

$sharedColumns1 = new ColumnDefinition();

$sharedColumns1->setName('Description');
$sharedColumns1->setId('cbb92da4-fd46-4c7d-af6c-3128c2a5576e');

$sharedColumnsArray []= $sharedColumns1;

$sharedColumns2 = new ColumnDefinition();

$sharedColumns2->setName('Address');
$sharedColumns2->setId('fc2e188e-ba91-48c9-9dd3-16431afddd50');

$sharedColumnsArray []= $sharedColumns2;
$documentSet->setSharedColumns($sharedColumnsArray);
$welcomePageColumnsArray = [];

$welcomePageColumns1 = new ColumnDefinition();

$welcomePageColumns1->setName('Address');
$welcomePageColumns1->setId('fc2e188e-ba91-48c9-9dd3-16431afddd50');

$welcomePageColumnsArray []= $welcomePageColumns1;
$documentSet->setWelcomePageColumns($welcomePageColumnsArray);

$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->patch($requestRequestBody);


```