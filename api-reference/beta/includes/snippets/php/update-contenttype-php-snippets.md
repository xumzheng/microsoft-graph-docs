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

$allowedContentTypesallowedContentTypes1 = new ContentTypeInfo();

$allowedContentTypesallowedContentTypes1->setId('0x0101');
$allowedContentTypesallowedContentTypes1->setName('Document');

$allowedContentTypesArray []= $allowedContentTypesallowedContentTypes1;
$documentSet->setAllowedContentTypes($allowedContentTypesArray);
$defaultContentsArray = [];

$defaultContentsdefaultContents1 = new DocumentSetContent();

$defaultContentsdefaultContents1->setFileName('a.txt');

$contentType = new ContentTypeInfo();
$defaultContentsdefaultContents1->setContentType($contentType);


$contentType->setId('0x0101');


$defaultContentsArray []= $defaultContentsdefaultContents1;

$defaultContentsdefaultContents2 = new DocumentSetContent();

$defaultContentsdefaultContents2->setFileName('b.txt');

$contentType = new ContentTypeInfo();
$defaultContentsdefaultContents2->setContentType($contentType);


$contentType->setId('0x0101');


$defaultContentsArray []= $defaultContentsdefaultContents2;
$documentSet->setDefaultContents($defaultContentsArray);
$sharedColumnsArray = [];

$sharedColumnssharedColumns1 = new ColumnDefinition();

$sharedColumnssharedColumns1->setName('Description');
$sharedColumnssharedColumns1->setId('cbb92da4-fd46-4c7d-af6c-3128c2a5576e');

$sharedColumnsArray []= $sharedColumnssharedColumns1;

$sharedColumnssharedColumns2 = new ColumnDefinition();

$sharedColumnssharedColumns2->setName('Address');
$sharedColumnssharedColumns2->setId('fc2e188e-ba91-48c9-9dd3-16431afddd50');

$sharedColumnsArray []= $sharedColumnssharedColumns2;
$documentSet->setSharedColumns($sharedColumnsArray);
$welcomePageColumnsArray = [];

$welcomePageColumnswelcomePageColumns1 = new ColumnDefinition();

$welcomePageColumnswelcomePageColumns1->setName('Address');
$welcomePageColumnswelcomePageColumns1->setId('fc2e188e-ba91-48c9-9dd3-16431afddd50');

$welcomePageColumnsArray []= $welcomePageColumnswelcomePageColumns1;
$documentSet->setWelcomePageColumns($welcomePageColumnsArray);

$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->patch($requestRequestBody);


```